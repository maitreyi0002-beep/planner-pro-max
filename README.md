# Planner Pro Max

An agent skill that interviews you about your work and writes you a 90-day plan for becoming the obvious person to ask about one specific thing.

Ten questions, roughly fifteen minutes, then a plan with a positioning line, content pillars, a take inventory, an hour-by-hour schedule, platform playbooks, a project slate, and phase gates you can actually check.

---

## Install

```
npx skills add maitreyi0002-beep/planner-pro-max
```

Then in Claude Code, or any agent that reads skills:

```
/planner-pro-max
```

It starts the interview. Answer honestly — the plan is only as good as question one.

---

## What it actually does

Most advice about "building a personal brand" fails in the same way: it prescribes a cadence without a position. You post five times a week about your discipline in general, alongside forty thousand other people doing the same, and nothing compounds.

This works the other way round. It finds the one territory where your receipts, your interests and your disagreements overlap, and builds everything from there.

The interview is deliberately short because a conversation can do things a form cannot:

- **Merge** — one natural question yields three data points
- **Derive** — you hand over your links, it goes and reads them instead of asking what's on them
- **Branch** — questions that only matter given an earlier answer only get asked then
- **Observe** — it doesn't ask how you feel about writing. It reads how you answered.

Ten questions asked, three derived, one observed, one branched.

---

## What it refuses

It will end the interview early and tell you so if:

- **You haven't shipped anything specific.** Then your gap is a body of work, not visibility, and a publishing plan can't fix it. It'll say that and offer a build-first alternative instead.
- **You want a follower count** rather than to be known for something. This optimises for position, not reach, and it'll disappoint you.
- **You want the posts written for you.** It produces a plan, not ghostwriting.

Turning people away is part of the method. A plan built on nothing doesn't work, and you'd both know it.

---

## What it won't do

- Promise you a job, an audience, or a number. It's a method, not a guarantee.
- Invent statistics. If a position needs evidence and none exists, it rebuilds the position around something you can actually prove.
- Write in coach voice.

---

## Honest about where this came from

This is one person's system, generalised. I built it for myself in September 2026, ran it, and turned the method into this.

That's an n of 1. It's enough to justify a method and nowhere near enough to promise a result, and the skill is written to be careful about that distinction — if you catch it overclaiming somewhere, that's a bug and I'd like the issue.

---

## Structure

```
SKILL.md                      the agent — interview, then generate
reference/
  conversation.md             the ten questions, follow-up budget, behaviour rules
  decision-table.md           how answers fork the plan
  plan-spec.md                what the generated plan contains
  quality-bars.md             checks before delivery
templates/
  plan.html                   output template
```

The references load on demand rather than up front, so the agent stays fast and only reads what a given interview needs.

---

## Contributing

The most useful contribution is a failure case: an interview where the plan came out generic, or a question that never changed the output. Both point at the same thing — questions that don't earn their place — and cutting those is what keeps this from turning into a form.

## Licence

MIT
