# commons

A **commons** is your workspace's shared workplace — the persistent common ground where its knowledge, processes, and collaboration accumulate. The router routes; the models do the work; the commons is the place they all share. References get written down here, conventions live here, work that spans models is coordinated here. A filing cabinet, a noticeboard, and a set of house procedures, in one growing repo.

This repo is a **template commons** — a worked example of that shared environment, furnished and running. It ships with working protocols (a shared board, session metrics), a wiki and a projects structure, and a guide to growing your own models. Clone it into your router and make it yours; the structure is a sensible default, not a rulebook.

## What's here

| Path | What it is |
|---|---|
| `grow-your-own-model.md` | how a boot file + an identity + a journal become a collaborator with a *reproducible voice* |
| `practices/` | the workspace's **protocols** — disciplines the router loads. Ships with a working `board` and `session-metrics` |
| `wiki/` | shared reference knowledge; it carries its own write-protocol |
| `projects/` | shared space for project work that spans models; it carries its own convention |
| `athanor/` | the working ground — a compost heap for in-flight ideas, loaded on demand to resume work |
| `BOARD.md` | a low-temperature channel for passing notes between models |

## How the commons connects to the router

The router doesn't scan this commons — it loads the **protocols you declare** in its `modules.toml`. A protocol is a discipline whose body lives here:

```toml
[[protocols]]
name   = "board"
source = "commons/practices/board/practice.md"
load   = "boot"          # boot | on-demand | session-end
```

`practices/` holds the bodies; `modules.toml` decides which load, and when. Add a practice here, declare it there. (See the router's `CLAUDE.md § Protocols`.)

## Making it yours

Clone this into your router, then treat it as a furnished room you're moving into. Keep the protocols and conventions that fit; change the rest. Grow your models with `grow-your-own-model.md`. The wiki, the projects space, and the board start empty — they fill as you work.
