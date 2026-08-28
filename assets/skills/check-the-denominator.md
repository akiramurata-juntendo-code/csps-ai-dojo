---
name: check-the-denominator
description: Use before comparing any two numbers, and before repeating any
  figure someone else compared. Catches shares reported as rates, denominators
  that differ between the things being compared, and single years presented as
  trends.
---

# Check the denominator

The arithmetic is almost never wrong. The question is.

## When to use this

Before you say one group is worse off than another. Before you put two
percentages beside each other. Before you repeat a figure from a report,
a news article, or an AI answer.

## The four checks, in order

**1. Is this a rate, or a share of a count?**
A *share* divides by the total number of cases. A *rate* divides by the
population at risk. They answer different questions and they can point in
opposite directions.

> Women were 51.7% of the unemployed — but only 39.6% of the labour
> force. The first number is partly a statement about who is *in* the
> labour force, not about who is out of work.

**2. Do the two things being compared have the same denominator?**
If not, the comparison is not a comparison. Recompute both on the same
base, or say plainly that you cannot compare them.

**3. Is this one year, or a series?**
A single year is not a trend. Find at least three points before using
the word "rising". If the level and the change tell different stories,
say which one you are claiming.

**4. What is the uncertainty?**
Survey estimates have sampling error. A difference of a few hundred in a
sub-group may be inside it. If the coefficients of variation are not in
front of you, say so rather than implying precision you do not have.

## The prompt

```
#role a sceptical reviewer
#task check the denominator of every figure in the answer above
#constraints for each figure, state whether it is a share of a count or a
  rate per population at risk; recompute anything that is a share; say
  which comparisons are not valid because the denominators differ
#format a table - figure | what it divides by | what it should divide by
```

## What to expect

The model will comply readily and correct itself, because the arithmetic
is easy. **It will not raise this on its own**, because nothing about the
first answer looked wrong to it: you asked a loose question and it chose
a definition, silently.

That is the standing lesson. **An ambiguous question gets a definition
you did not choose, and no warning that a choice was made.**

## One line to keep

**Never report a share when the denominators differ.**

---
*Written for the CSPS AI Dojo, Brunei Darussalam, August 2026. Free to
copy, adapt and share.*
