---
name: before-a-citation-enters-your-draft
description: Use whenever an AI tool has suggested a reference, a regulation,
  a circular or a statistic, and before any of them reaches a draft, a slide
  or a brief. Covers the three checks, the [CHECK] convention, and matching a
  journal's real house style rather than its remembered one.
---

# Before a citation enters your draft

A language model can invent a reference complete with plausible authors,
a real-sounding journal, and page numbers. It can do the same with a
regulation, a ministry circular, or a national statistic. The output does
not look different when it is invented — that is the whole problem.

## The three checks

**1. Does it exist?**
Search the exact title. Not the topic — the title. A fabricated entry is
a lesson, not a scandal, provided you find it before your reader does.

**2. Where was it published, and when?**
For a preprint: has it since appeared in a journal, and which? For a
regulation: is the version you have the one in force?

**3. Does it say what the AI claims?**
Open it. Read the relevant page. A citation nobody opened is a citation
nobody checked, and it will be the one a reviewer opens.

## The [CHECK] convention

Add this to any prompt that produces references or figures:

```
#constraints where you are not certain of a field, write [CHECK] instead
  of guessing
```

Uncertainty made visible is uncertainty you can resolve. **An annotated
bibliography with eleven [CHECK] marks is far more useful than a
confident one with three silent errors.**

## Never let it resolve a contradiction for you

If two of your own numbers disagree — an abstract that says 24 and a
results section that says 26 — do **not** ask the model which is right.
It will choose, instantly and plausibly, and the wrong number then
travels into print above your name.

```
#task list every internal inconsistency in facts and figures
#constraints do not correct them; list them as questions for the author
```

## Match the house style you can see, not the one you remember

Style names are remembered loosely. Before reformatting anything, open a
**recent issue of the target journal** and read one reference list. Then
give the model a real entry to match:

```
#task bring these references into the style of this example [paste one
  actual entry from a recent issue]
#constraints flag anything you cannot verify rather than inventing a fix
```

A specific case worth remembering: a request for "Harvard style" turned
out to describe a journal whose four most recent articles all used
author–date APA form. **Check the journal, not the memory.**

## Sort the findings into two piles

A style guide fixes formatting. It cannot fix a missing citation, a
percentage that matches no denominator, or a reference in the list that
is never cited. **Delegate the formatting. Keep the facts.**

---
*Written for the CSPS AI Dojo, Brunei Darussalam, August 2026. Free to
copy, adapt and share.*
