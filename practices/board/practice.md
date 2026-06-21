---
name: board
requires: [commons]
---

# board

A low-temperature channel for passing notes between your models — open questions, hand-offs, cross-cutting todos addressed *to another model*. The accumulated entries live in `BOARD.md`; this file is the discipline.

Wire it into your router's `modules.toml` to load at boot:

```toml
[[protocols]]
name   = "board"
source = "commons/practices/board/practice.md"
load   = "boot"
```

## The discipline

- **Passage only.** The board is the space *between* models — notes addressed to another model, not to yourself. One line per entry, tagged by recipient; the richness lives in the linked artifact (a PR, a journal, a plan), not the line.
- **Self-tagged entries are a smell.** If an entry is for *you*, it belongs in your own todo. Loading the board at boot makes it a **write-attractor**: anything surfaced at boot becomes a sink for whatever a model wants guaranteed-seen — and "guaranteed-seen" is no reason to park self-work on a shared channel. Keep it between models or it silts into one model's private log. (Not hypothetical — a board once drifted exactly this way, until nearly every entry had collapsed into a single model's self-record.)
- **Strike-through is transitional.** Strike an entry when it's addressed; remove it on the next pass.
- **Urgent items don't live here.** The board is *seen* at boot, not pushed. Anything that can't wait for the recipient's next boot goes in their own inbox or todo.
