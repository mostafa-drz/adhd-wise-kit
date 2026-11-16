# Skill lab

No skill ships, and no skill change merges, until it passes the lab. The lab exists to raise
the bar: fewer, better skills that work on the first reply for a real adult with ADHD.

## The loop

1. **Simulate.** For each persona in `personas/`, the `lab-simulator` agent runs a short,
   realistic session: the persona's opening message, the skill's replies (strictly following
   the skill's `SKILL.md`), and the persona's honest reactions. It writes the transcript.
2. **Review, independently.** Three reviewers score every transcript against `rubric.md`
   without seeing each other's scores:
   - `reviewer-lived` reads as an adult with ADHD: would this help me right now?
   - `reviewer-evidence` checks the technique against research and the safety rules.
   - `reviewer-ux` checks the first 5 seconds, load, setup friction and the path back.
3. **Debate and decide.** The lead (the main session) puts disagreements side by side, asks
   each reviewer to answer the strongest point against them once, and records the verdict.
4. **Fix and re-run.** Every "fail" becomes a concrete `SKILL.md` change in the same PR. Re-run
   the failing personas until the skill passes.

## Bar to ship

- Every criterion averages **4 or more out of 5** across personas and reviewers.
- **No red flag** from any reviewer (safety, shame, a claim we can't back, an action without
  consent).
- The first reply always gives one next step with a time, in under 60 words.

Reports go in `reports/<skill>-<YYYY-MM-DD>.md`: transcripts, scores, the debate, the verdict
and the changes made. Personas are fictional composites; never put real people's details here.
