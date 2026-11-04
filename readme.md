# System Design Task: Product Catalog Service

## The task

Design a system that does all of the following:

1. **Receives "Product Catalog Updates" from suppliers.**
2. **Exposes the catalog through a "Public API"** used by user apps.
3. **Updates downstream "Internal Services"** (for example, analytics) when products change.

You don't need to design the Public API or the Internal Services themselves. They are consumers of your service.

## Estimated numbers

**Product catalog**
- 500 suppliers
- ~5M unique products
- Updates arrive via HTTP webhooks at an uneven pace: some suppliers send a few times a day, with bursts of up to ~50 updates/s

**Public API**
- ~2k requests/s sustained, read-only

## What we'd like from you

- **Visualise the architecture** however you prefer: boxes and arrows, any drawing tool, or just describe it. Neat diagrams are not required.
- **Say what you skip, what you postpone, and what you guess or assume.** There is no hidden "correct" answer, and we're more interested in your reasoning than in completeness.
- **Think out loud and ask questions** whenever something is unclear. We'll play the role of the business and answer as best we can.

## How it works

- **Time:** about 25 minutes in total.
- **Start:** take 3 to 5 minutes to read and think before you start drawing.
- **Afterwards:** we'll talk about your design together and may change some of the assumptions.
