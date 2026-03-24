---
sidebar_position: 20
sidebar_label: "Extension: Decision Trees"
title: "Extension Week 2: Decision Trees"
description: "Mapping complex, multi-step decisions with branching paths, probabilities, and working backwards."
---

# Extension Week 2: Decision Trees
*Mapping Complex, Multi-Step Decisions*

Most of the decisions in this course have been single-step: "Should I do X or Y?" But real life is often more complex. One decision leads to another, which leads to another. **Decision trees** let you map out these branching paths, see all the possible futures, and work backwards from where you want to end up.

This is the tool of choice for strategists, doctors making treatment plans, and anyone facing a sequence of interconnected choices.

---

:::info Caregiver Snapshot
- Decision trees are visual and hands-on — lots of drawing this week.
- The concept of "working backwards" is especially powerful and applies far beyond decision trees.
- This extension works best after the student has mastered Expected Value (Week 9).
- Target age: best for ages 9+ or advanced younger students.
:::

:::tip Quick Navigation
- [Teacher Preparation](#teacher-preparation)
- [Guided Session 1: The Decision Tree](#guided-session-1)
- [Guided Session 2: Working Backwards](#guided-session-2)
- [Independent Session](#independent-session)
:::

## Teacher Preparation

:::info Before You Begin
- Large paper or poster board for drawing trees (they spread out!)
- Colored markers (one color per decision branch works well)
- Prepare the Practice Scenario trees (partially drawn for the student to complete)
- Review Expected Value (Week 9) — we combine EV with trees this week
:::

:::tip Teaching Mindset
Decision trees look complicated but they're just a series of what-if questions drawn out. Start very simple and build up. If the student gets overwhelmed, zoom in to just one branch at a time.
:::

---

## Guided Session 1
### The Decision Tree
#### Learning Goal
By the end of this session, the student can:

- draw a decision tree for a 2-step decision
- distinguish between decision nodes (you choose) and chance nodes (the world decides)
- read a decision tree to compare different paths

---

#### Activities

**1. Anatomy of a Decision Tree**

Draw the basic elements:

```
■ = Decision Node (YOU choose)
● = Chance Node (the WORLD decides)
▶ = Outcome (what happens)
```

Simple example:

```
■ Bring an umbrella?
├─ YES (bring it)
│   ● Weather?
│   ├─ Rain (60%) → ▶ Dry and prepared! [Score: 8]
│   └─ Sun (40%) → ▶ Carried it for nothing [Score: 5]
│
└─ NO (leave it)
    ● Weather?
    ├─ Rain (60%) → ▶ Soaking wet! [Score: 2]
    └─ Sun (40%) → ▶ Free hands, sunshine! [Score: 9]
```

Now calculate the Expected Value of each branch:

- **Bring umbrella:** (0.6 × 8) + (0.4 × 5) = 4.8 + 2.0 = **6.8**
- **No umbrella:** (0.6 × 2) + (0.4 × 9) = 1.2 + 3.6 = **4.8**

Conclusion: Bring the umbrella! (Higher EV)

But notice: the BEST single outcome is leaving the umbrella on a sunny day (score 9). The tree tells us to give up the best-case scenario to avoid the worst-case scenario. That's the power of EV + trees together.

---

**2. A Two-Step Tree**

Now add a second decision:

```
■ Study for the test?
├─ YES (study 1 hour)
│   ● Test result?
│   ├─ Pass (85%) → ■ Celebrate or study more?
│   │                  ├─ Celebrate → ▶ Happy, good grade [8]
│   │                  └─ Study more → ▶ Very prepared for next test [7]
│   └─ Fail (15%) → ■ Try again or give up?
│                     ├─ Try again → ▶ Learning from failure [5]
│                     └─ Give up → ▶ Defeated feeling [2]
│
└─ NO (play instead)
    ● Test result?
    ├─ Pass (30%) → ▶ Lucky! Free afternoon AND good grade [9]
    └─ Fail (70%) → ■ Try again or give up?
                     ├─ Try again → ▶ Behind but trying [4]
                     └─ Give up → ▶ Failed and behind [1]
```

Discuss:
- "See how one decision leads to another? The tree shows ALL possible futures."
- "Which overall path gives the best expected outcome?"
- Calculate the EV of the "Study" branch vs. the "Don't Study" branch.

---

**3. Build a Tree Together**

Choose a fun scenario and draw a tree from scratch:

Suggested: "It's Saturday morning. You can go to a friend's house OR stay home and play video games. But if you go to your friend's house, you might get invited to go swimming (which you love) OR you might end up doing something boring."

Draw it out:
- What are the decision nodes?
- What are the chance nodes?
- What probabilities and scores would you assign?
- What does the tree recommend?

---

## Guided Session 2
### Working Backwards
#### Learning Goal
By the end of this session, the student can:

- use "backward induction" to find the best path through a multi-step tree
- explain why starting from the end is sometimes easier than starting from the beginning
- apply working-backwards thinking to a real scenario

---

#### Activities

**1. The Maze Strategy**

Quick warm-up:

> "When you solve a maze, is it easier to start from the beginning or the end?"

Many mazes are MUCH easier solved backwards because from the end, there's often only one path. From the start, there are many branches.

> "Decision trees work the same way. Start at the end (the outcomes), and work backwards to figure out the best first move."

---

**2. Backward Induction**

Return to the two-step study tree from Session 1. Solve it from the bottom up:

**Step 1: Solve the last decisions first.**

At each final decision node, pick the better option:
- "Celebrate or study more?" → Celebrate (8 > 7)
- "Try again or give up?" after studying → Try again (5 > 2)
- "Try again or give up?" after not studying → Try again (4 > 1)

**Step 2: Replace each final decision with its best value.**

Now the tree simplifies:

```
■ Study?
├─ YES → (0.85 × 8) + (0.15 × 5) = 6.8 + 0.75 = 7.55
└─ NO → (0.30 × 9) + (0.70 × 4) = 2.7 + 2.8 = 5.5
```

**Step 3: Choose the first move with the highest value.**

Study wins (7.55 > 5.5).

> "By solving from the end, we figured out the best strategy for every possible future FIRST, then used those answers to make the first decision. This is called **backward induction** and it's how chess players, business strategists, and game designers think."

---

**3. Plan a Strategy Game**

Apply backward thinking to a simple strategy game:

**The Counting Game:**
- Two players take turns.
- On your turn, say 1, 2, or 3 numbers (continuing the count upward).
- The person who says "21" loses.

Play a few rounds. Then:

> "Can you figure out the winning strategy? Work backwards from 21."

- If you say 21, you lose.
- So you want your opponent to say 21.
- If you say 20, they must say 21. You win!
- So you want to say 20. To guarantee saying 20, you need to say 16 (they say 17-19, you say 20).
- To guarantee 16, say 12. Then 8. Then 4.
- **Winning strategy: say 4, 8, 12, 16, 20. (Multiples of 4!)**

> "By working backwards from the end, you can figure out the exact winning strategy. This is backward induction in action!"

---

**4. Real-Life Working Backwards**

Apply the technique to a real goal:

> "Where do you want to end up? Now let's work backwards to figure out what decisions you need to make."

Example:

```
GOAL: Finish a big school project without stress (due Friday)

  What needs to be true on Thursday night? → Project is almost done
  What needs to happen by Wednesday? → First draft is complete
  What needs to happen by Tuesday? → Research is done
  What needs to happen by Monday? → Topic is chosen, materials gathered
  What should I do TODAY (Sunday)? → Choose topic and make a plan
```

> "Instead of staring at a big goal and feeling overwhelmed, working backwards breaks it into clear steps."

---

## Independent Session

### Goal

Build decision trees for real decisions and practice backward thinking.

### Activities

**1. My Decision Tree**

Pick a real decision you're facing (or one coming up soon). Draw a full decision tree:

- At least 2 decision points
- At least 2 chance nodes with estimated probabilities
- Score each outcome (1-10)
- Calculate the EV of each main branch
- Use backward induction to find the best first move

**2. Goal Backwards**

Pick a goal you want to achieve in the next month. Work backwards from the goal to today:

- What needs to be true the day before the deadline?
- What needs to happen the week before?
- What should you start doing THIS week?
- What's the very first step?

### Decision Journal

> Draw a decision tree for an important upcoming choice. Include probabilities and outcome scores. What does the tree recommend? Does the recommendation match your gut feeling? If they disagree, which will you follow and why?

### Reflection Questions

- When is a decision tree overkill? When is it worth the effort to draw one?
- Is it better to plan every step in advance, or to figure things out as you go? When does each approach work best?
- Can you think of a game (board game, video game, or sport) where "working backwards" would help you win?
