# future-self

**The one question that stops most bad decisions - and a five-stage exercise for when the answer dodges.**

> Will my future self thank me for this?

If you can answer that in one clear sentence, you don't need this skill. If your answer starts with *"probably"*, *"I think so"*, or *"it depends"* - that dodge is the signal. It means impulse and coherence are currently indistinguishable, and this is the tool that separates them.

`future-self` is a decision-coherence exercise for **personally consequential decisions**: take the job? move? quit? commit to the two-year thing? It does not score your options or predict outcomes. It examines *you* - your motives, your patterns, your history - and hands you the conditions under which either choice would be self-respecting.

## What it is not

- **Not a recommender.** It never says "you should". It says "Scene A produces more calm, self-respect and room to move - given your own record."
- **Not a premortem.** A premortem stress-tests the *plan* (what could make it fail). `future-self` examines the *decider* (why you want it, and what that wanting is made of). Big decisions deserve both.
- **Not a vibe check.** Fear can precede a good decision because it's new. Euphoria can make a bad one attractive. The exercise treats your gut as data, not verdict.

## Quickstart

### Claude Code

**Option A - Plugin marketplace:**

```
/plugin marketplace add marmbiz/future-self
/plugin install future-self@future-self
```

**Option B - Manual (any setup):**

```bash
git clone https://github.com/marmbiz/future-self.git
cp -r future-self/skills/future-self ~/.claude/skills/
```

Then, in any session:

```
/future-self should I take the offer in Marktoberdorf?
```

### OpenAI Codex CLI

```bash
git clone https://github.com/marmbiz/future-self.git
cp future-self/codex/future-self.md ~/.codex/prompts/
```

Then invoke with `/future-self <your decision>` inside Codex.

## What happens when you run it

**Stage 0 - The One Question.** You get asked the question, verbatim. A clear answer ends the session in a paragraph - decisions that carry themselves in one sentence don't need a program. An evasive answer starts the exercise.

**Grounding.** The exercise is worthless without the person. If you use persistent memory, the skill reads your documented patterns, hard criteria and past decisions. If not, it asks four questions first - and waits. No exercise on placeholders.

Then, five stages:

| Stage | What it does | The question it answers |
|---|---|---|
| **1. Strip-Down Test** | Removes short-term reward, fear, recognition and time pressure - one layer at a time, evidenced with your own history | How much of this is impulse, how much is coherence? |
| **2. Burden Ledger** | What future-you carries vs. what future-you gets | Would I knowingly put this on them? |
| **3. Two Scenes** | Two prose scenes, months in: you did it / you didn't | Which produces more calm, self-respect, room to move - *after* the first emotional spike? |
| **4. No-Defense Test** | Both versions explained to a friend who isn't buying and doesn't need impressing | Which version needs lawyers? *(Evidence explains itself. Feelings need justifications.)* |
| **5. Kill Criteria** | 3-5 pre-defined, observable walk-away signals - external and internal | If I walk later, was it a decision or my old pattern? |

The deliverable is Stage 5. Most decision tools end with a verdict; this one ends with **kill criteria** - so that if you do walk away later, it's a conscious decision you defined in advance, not the pattern catching up with you. The skill offers to persist them into your project notes, because kill criteria nobody can find later falsify nothing.

## Who this is for

People who keep re-litigating the same decision at 11 pm. People with a documented retreat pattern they'd like to stop obeying blindly. People whose problem is not a lack of analysis, but too much of it - and no way to tell which part of the wanting is real.

It works best if the assistant knows you (persistent memory with your patterns and past decisions). It still works cold - it will just interview you first.

## Design principles

1. **No recommendation, ever.** Autonomy is the point. The tool describes; you decide.
2. **Evidence over psychology.** Your own past decisions are the proof material - not frameworks.
3. **The uncomfortable parts are mandatory.** Known patterns, rationalizations and overridden criteria get named. No cheerleading.
4. **Prose where it matters.** The Two Scenes and the No-Defense Test are written as prose. You cannot feel a bullet point.
5. **Both answers can be self-respecting.** The exercise defines the conditions for each - that's the whole trick.

## Origin

Built from a simple observation: *"Will my future self thank me for this? If the answer is somehow evasive - think again."* The five stages exist for exactly that second case. First used in the wild on a real decision (a two-year leadership role, a small town, a life somewhere else entirely) - the kill criteria from that session ended up next to the interview notes, where they belong.

## License

MIT
