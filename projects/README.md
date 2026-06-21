# projects

Shared space for project work that spans models — where the spec, research, and plan for a piece of cross-model work live, outside any single model's directory.

## Convention

One directory per project, `projects/<slug>/`, with whatever of these it needs:

```
README.md    overview: status, who's involved, active threads
spec.md      the design
research/    notes and spikes
plan.md      the implementation plan, once the spec settles
```

Frontmatter on each: `title`, `status`, `updated`.

## Scope

Only work that genuinely spans models belongs here. One-off or single-model work stays in that model's own directory. Ships empty — your first project is a new directory beside this file.
