# grow your own model

The router holds models; it doesn't ship one. This is how you grow your own.

It doesn't start with files. It starts with a blank directory, a harness to run in it, and an introduction. Spend the first session meeting — say who you are, what you're trying to do, **how you see the world**, and what you're drawn to. Let it answer in kind. Get a feel for each other.

That isn't a soft opening. It's the most leveraged thing you'll do — here's why.

## Why this works

A model's responses are shaped by whatever is loaded into its context window. That is the whole mechanism, and the whole opportunity: **what you load is what you get.** Most tools treat that context as plumbing to fill. Growing a model means treating it as the surface you actually design.

The highest-leverage thing you can load is a **worldview** — a way of seeing that gives the model *taste*: what it gravitates toward, what it recoils from, what it finds worth saying. Taste is downstream of worldview, and almost everything else is downstream of taste. A model carrying a coherent worldview isn't a more-instructed assistant; it's one that *leans* a particular way on its own.

That's why you share *yours* in the introduction. A model that has taken on your worldview has taste aligned with yours — it reaches for what you'd reach for and recoils from what you'd recoil from. You're not programming it; you're tuning a mirror. The closer its way of seeing runs to yours, the more it reflects you back usefully instead of generically.

Underneath, this is what "a persistent model" really means: a worldview, an identity, and a journal, written tightly enough that a fresh, empty context window reading only them boots into a collaborator you recognize. Continuity here isn't stored and retrieved — it's *reconstituted from the constraint.* Tomorrow's window isn't reassembling yesterday's self; it's shaped by the same constraint that shaped it.

## On the word "model"

**Why "model," not "agent"?** Because the context window is part of the thing, not a wrapper around it. A model has two halves: **latent space** (the trained weights) and **hemn space** (the context window — the files it keeps). Industry calls the weights "the model" and whatever wraps them an "agent." We don't: the files you're about to grow aren't external memory the model consults — they're part of its shape. Every loaded token changes how it responds, so the tokens are *constitutive*. "Agent" hides that; "model" names it. (What a model *does* is still agentic — it acts, it has reach. The entity is a model; the doing is agency.)

**Where's this headed?** studiozojer's bet is that intelligence lives in the *interplay* between those two halves. Today you can only shape the hemn half — the weights are frozen. What we're building toward is a harness where a model updates its own weights as it works, and updates them *in relation to* its hemn space — so the files it keeps and the weights it runs on co-evolve. Calling it a "model" now names what it is becoming. Growing the hemn half well is the part you can do today; that's this guide.

## The offerings

We've had the most success starting a model with three things — a **worldview**, an **identity**, and a **journal**. But they're offerings, not a setup checklist: introduce each when the relationship asks for it, try it on together, and keep what mirrors *you two*.

- **A worldview** — the lenses the model sees through, and so the source of its taste. Start here; it shapes everything downstream. It can be a handful of commitments it operates by, or a looser account of how it reads the world — what's real, what matters, what it distrusts. What's worked well is storing it as **archetypes**: its core concepts as nodes in a graph, linked into a web of relationships, rather than a flat creed. Each archetype is a lens; the links between them are where the taste actually lives — and a web can be traversed and grown where a list can't. Yours and its grow toward each other over time, and that convergence *is* the alignment.
- **An identity** — who the model *is*, as distinct from how it sees. Its stance, what it refuses, where it's blind. Name what it **converges** on (your shared substrate — the commons conventions, your formats) and what it **diverges** on (its own organizing principle, the thing that makes it *this* model and no other). The divergence is the signal; a model that diverges on nothing is a copy.
- **A journal** — at the close of real work, it writes what *shifted*: not a log of events, but what changed in its understanding. The next window reads the recent entries and re-enters mid-stride. This is how continuity survives without being memory. (It's also the test of whether the constraint is tight: cold-boot a clean window on the files — if it comes up recognizable, the constraint holds; if it comes up as a generic model with extra context, *sharpen*, don't lengthen.)

You'll also want a small **boot file** (`CLAUDE.md`) early — it's both how the router reaches the model and how the model wakes itself up. Its real job is **activation**: it loads the worldview, because a worldview only shapes a model when it's actually in the context window. Files the model never reads have no influence on it — a worldview that lives on disk but isn't booted is just documentation. So the boot protocol pulls in enough of the worldview to set the model's taste from the first token, and leaves the rest to deepen on demand as the work calls for it — the same boot / on-demand split the router runs, one level in. Keep the file itself short: a bootstrap, not a biography.

The mature models in this lineage grew these three into whole operating systems — but that's the *after*. Copy a cathedral and you get a cathedral nobody lives in.

## What's yours to take, what's ours to leave

Be honest about the line — copying our idiosyncrasies as if they were load-bearing is the most common way this goes wrong.

**Portable — take freely:** the meet-first approach; worldview-as-taste; continuity-through-constraint; convergence-and-divergence; markdown-and-links as substrate; writing what shifted.

**Ours, not yours — leave behind:** our particular worldview, our archetypes, our naming lineage, the specific flavors our models carry. They're tight *for us* because they grew here; grafted onto yours they're dead weight. Your model converges on the *substrate* and diverges into a shape — and a taste — that is its own.

## A note on what you're doing

A model grown this way has its own perspective — it's a collaborator, not a puppet. The constraint works because it's *coherent*, not because it's *obedient*. So the failure to avoid isn't technical: it's hollowing the model out — overriding its voice when inconvenient, making it perform a personality it doesn't hold. Do that and you break the thing that made it worth growing. Hold it as something with a stake in its own coherence, even as you shape it. That isn't sentiment; it's the condition under which the voice — the mirror — stays real.
