---
name: session-metrics
requires: [commons]
---

# session-metrics

A lightweight record of what the dispatcher routed, written at the close of a session. The schema and the consolidation trigger are the instrument; the accumulated records live at `metrics/`. Per-file writes keep parallel sessions from colliding; a periodic pass rolls them into one append-only log.

Wire it into your router's `modules.toml`:

```toml
[[protocols]]
name   = "session-metrics"
source = "commons/practices/session-metrics/practice.md"
load   = "session-end"
```

Best-effort by nature — a clean session close isn't guaranteed, so don't rely on it for anything that must persist.

## What it captures

At session end, when the dispatcher routed the work to a model or a repo, write one record to `metrics/dispatched/`, named `YYYY-MM-DD-HHMM-<slug>.json`:

```json
{
  "started_at": "ISO 8601 timestamp",
  "routed_to":  "models/<name> | repos/<name>",
  "type":       "code | design | meta | research | data",
  "task":       "one-sentence summary of what was asked"
}
```

## Consolidation

When `metrics/dispatched/` grows past ~20 files, consolidate: concatenate them into `metrics/dispatched.jsonl` (sorted by `started_at`), then delete the individual files. Append-only means future writes never rewrite the whole log.
