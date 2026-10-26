# AGENTS.md

Instructions for any agent working in this repository.

## The entry point

`README.md` is the live status of the project. Every session starts by reading it and ends by updating it. Its "Current state", "Milestones", and "Decision log" must be true at the end of any work — not aspirational.

## What must never drift

1. **Numbers.** Every figure is either sourced (`[F]`, with a citation resolving in `Project-H-Market-Intelligence-Report.md` §16.2), a target (`[T]`), or the customer's own measurement (`[C]`). Never invent revenue, share, complaints, specs, completion rates, or clinical performance. If a number is not measured, label it.
2. **The stage block.** "Pre-pilot. No product, no revenue, no clinical advisor, no company." This exact state appears in every customer-facing document until it is factually no longer true. One document claiming more than another kills the pack.
3. **The claims ladder.** `Project-H-Master-Plan.md` §11.2 defines what may be said at each evidence stage. Anything customer-facing or investor-facing must sit at or below the current stage. Default to the lower-stage sentence.
4. **The clinical boundary.** The clinician decides. This product does not diagnose, advise, prescribe, or interpret readings clinically. No document, pitch, feature, or script may blur that line, regardless of what a customer asks for.
5. **The send order.** Clinic (`pitch/01`) → advisor (`pitch/03`) → grant (`pitch/02`) → investor (`pitch/04`). Do not recommend an earlier send.

## House structure

| File | Answers | Do not duplicate its content elsewhere |
|---|---|---|
| `README.md` | What is true right now, and what is next | — |
| `Project-H-Master-Plan.md` | The vision, trajectory, org, capital, weekly room | Trajectory and strategy |
| `Project-H-Market-Intelligence-Report.md` | The evidence and its quality | Sourcing and market sizing |
| `Founder-Playbook-Bootstrap-India.md` | Operations with no capital | Week-by-week execution |
| `pitch/` | Four audiences, one evidence base | Audience-specific wording |

New material should extend one of these, not create a sixth document that restates them.

## Writing style in this repo

Plain English, short sentences, tables over paragraphs, no superlatives, no "revolutionary", no "AI" unless there is a model. If a claim cannot survive "how do you know that?", delete it.

## When a session changes the plan

1. Update the affected document.
2. Append one line to the README decision log with the reason.
3. Update `README.md` "Current state" if stage, revenue, sites, or patients changed.
4. If the stage changed, check the claims ladder before anything customer-facing goes out.
