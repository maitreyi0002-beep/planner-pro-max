# Examples

Empty on purpose, for now.

The first worked example should be a real interview, not an invented one. A fabricated example teaches the agent to produce fabricated-looking plans, and anyone reading this repo can tell the difference between a transcript and a mock-up.

## What to put here

For each real run, with the person's permission and identifying details removed:

```
examples/
  run-01/
    transcript.md     the interview as it actually went
    plan.html         what came out
    notes.md          what you'd change
```

`notes.md` is the one that matters. For each run, record:

- **Which questions changed the output**, and which didn't
- **How many follow-ups** you needed before you could write the plan
- **Anything you had to ask that isn't in the ten** — that's a missing question
- **Where the plan came out generic** — that's a failing question

After about twenty runs, those notes tell you which questions to cut. That's the path from this being a conversation someone runs to something that can run itself.

## The first one should be yourself

Run the interview on your own work, honestly, and see whether the plan it produces resembles the one you'd write by hand. If it doesn't, the ten questions are missing something — and finding that out on yourself is far cheaper than finding it out on a customer.
