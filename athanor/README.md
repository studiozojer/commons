# athanor

The athanor is your workspace's **working ground** — the hot, in-progress space where ideas accumulate before they're ready to be anything. If the wiki is the finished reference and a model's journal is its settled memory, the athanor is the **compost heap**: the big pile of half-formed tokens you're still turning over.

## Why it exists — compost

Good work throws off far more good ideas than you can use at once. You don't want to throw them away — they're worth something. But you don't want to hold them too tightly either — an idea gripped too early hardens into the wrong shape. The athanor resolves that tension: a big ball of tokens you can let sit, sort through, pick and choose from, and **refine into lasting shapes — a wiki page, a project, a model's identity — only when they're ripe.** Until then, they compost.

The discipline is mostly about *not* doing things:

- don't throw a good half-idea away — drop it in the athanor;
- don't force it into final form before it's ready — let it sit;
- when it's ripe, fold it out (into the wiki, a project, wherever it belongs) and let the husk go.

Nothing in here is precious, and nothing in here is the record of anything — the canonical version always lives somewhere cooler. The athanor is *allowed* to be a mess; that's the job.

## Using it

It's a normal directory you load into when you want to pick up in-flight work. A **briefing** (`briefing.md`) is the front door — a light, current note of what's cooking — so a fresh window, or a parallel one, can resume where the last left off. Keep the briefing committed; everything else in here is loose working files you sort as you go.

We're still finding the right shape for this ourselves, so it's deliberately light. Use it however helps; it'll sharpen with practice.

## Wiring it into the router

The athanor loads **on demand** — you enter it when you want it, not every session:

```toml
[[protocols]]
name   = "athanor"
source = "commons/athanor/briefing.md"
load   = "on-demand"
when   = "the user wants to resume or work in the athanor"
```

When you reference it, the dispatcher reads the briefing and you pick up the working context — from your last session, or from a parallel window that committed it. (It picks up the last *committed* state — windows sync by commit and pull, not in real time, so commit the briefing often.)
