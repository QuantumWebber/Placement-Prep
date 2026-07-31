# CRED — Online Assessment Experience (Round 1)

> Interview experience log for my placement prep repo. Sharing this so the next batch walks in prepared instead of guessing.
> **TL;DR:** Round 1 was heavily graph-flavoured, half of it was *debugging* (not writing from scratch), and DP barely showed up.

---

## Round Structure

| Round | Format | Focus |
|---|---|---|
| **Round 1 — Online Assessment** | 4 DSA questions: **2 debugging + 2 coding** | Graphs, greedy/math, multi-source BFS/DFS |
| **Round 2** (reported) | LLD / machine coding | Low-level design, OOP, class modelling |
| **Round 3** | Technical Interview | Projects + DSA + fundamentals |

---

## Round 1 — Detailed Breakdown

### Section A: Debugging (2 questions)

Buggy code is given, you fix it. Logic samajhna is the whole game here — you can't brute-force your way through, you have to actually read someone else's code and spot where the invariant breaks.

**Q1 — Domino Parity (~15 marks, easier one)**

Dominoes numbered `1` to `6`. Each domino is split into two parts (two numbers). A domino is "valid" when the **sum of its two parts is even**. You're allowed a **rotation operation** that rotates the digits of a domino to try and make the sum even.

**Goal:** minimum number of rotation operations to make every domino valid.

*Core insight:* parity. Sum is even only when both parts are odd or both are even. So it reduces to counting odds/evens per position and figuring out the cheaper of the two target states — a classic "make all elements equal with min ops" pattern in disguise.

**Q2 — Grid Graph Traversal (harder one)**

A variety/hybrid problem built on top of standard grid-graph patterns — think **Rotting Oranges** and **Pacific Atlantic Water Flow** stitched together. The key requirement was **multi-source BFS/DFS** handled across **multiple test cases** (state reset between cases is where the planted bug usually lives).

If you know these two patterns cold, this is a 10-minute question. If you don't, it's unsolvable in the time given.

---

### Section B: Coding (2 questions)

Exact problems I don't remember, but **at least one was a graph problem**. Consistent with the debugging section — this OA was graph-weighted end to end.

---

## What Actually Mattered

**High priority**
- Graphs — BFS, DFS, multi-source BFS, grid traversal, connected components, reverse-traversal-from-boundary
- Grid/matrix simulation problems
- Parity, math-greedy, "minimum operations to make X uniform" patterns
- **Reading and debugging other people's code** — an underrated skill nobody practices

**Low priority**
- **DP was not important for this round.** Don't over-invest here at the cost of graphs.

---

## Similar Questions to Practice

Do these before your OA. The debugging section is basically these problems with bugs planted in them.

### Grid BFS / Multi-source
- [994. Rotting Oranges](https://leetcode.com/problems/rotting-oranges/)
- [417. Pacific Atlantic Water Flow](https://leetcode.com/problems/pacific-atlantic-water-flow/)
- [130. Surrounded Regions](https://leetcode.com/problems/surrounded-regions/)
- [1020. Number of Enclaves](https://leetcode.com/problems/number-of-enclaves/)
- [542. 01 Matrix](https://leetcode.com/problems/01-matrix/)
- [1091. Shortest Path in Binary Matrix](https://leetcode.com/problems/shortest-path-in-binary-matrix/)
- [286. Walls and Gates](https://leetcode.com/problems/walls-and-gates/) (premium)
- [934. Shortest Bridge](https://leetcode.com/problems/shortest-bridge/)

### Core Graph
- [200. Number of Islands](https://leetcode.com/problems/number-of-islands/)
- [207. Course Schedule](https://leetcode.com/problems/course-schedule/)
- [133. Clone Graph](https://leetcode.com/problems/clone-graph/)
- [547. Number of Provinces](https://leetcode.com/problems/number-of-provinces/)
- [127. Word Ladder](https://leetcode.com/problems/word-ladder/)

### Parity / Min-Operations / Greedy-Math
- [1007. Minimum Domino Rotations For Equal Row](https://leetcode.com/problems/minimum-domino-rotations-for-equal-row/) ← closest analogue to Q1
- [453. Minimum Moves to Equal Array Elements](https://leetcode.com/problems/minimum-moves-to-equal-array-elements/)
- [462. Minimum Moves to Equal Array Elements II](https://leetcode.com/problems/minimum-moves-to-equal-array-elements-ii/)
- [1042. Flower Planting With No Adjacent](https://leetcode.com/problems/flower-planting-with-no-adjacent/)

---

## Give LeetCode Weekly Contests — Seriously

Sheets se pattern aa jaata hai, **speed nahi aati**. And OAs are scored on speed under pressure, not on whether you *eventually* got it.

Why contests are non-negotiable:

1. **Time pressure is a separate skill.** Solving Rotting Oranges in 40 relaxed minutes ≠ solving it in 12 minutes with a timer running.
2. **You get unlabelled problems.** No "Graphs" tag above the question. OAs are exactly this — pattern recognition from a raw statement.
3. **Contest Q2/Q3 ≈ OA difficulty.** That's the actual band product-company OAs sit in.
4. **Upsolving is where growth happens.** Solve what you couldn't within 24 hours while the frustration is still fresh. That memory sticks.
5. **Debugging under a clock.** Your own WA-on-testcase-47 panic is the same muscle the debugging section tests.

**Suggested cadence:** Weekly Contest (Sunday) + Biweekly (alternate Saturdays) + upsolve every unsolved question the next day. Even 2 contests a month for 3 months changes your ceiling completely.

---

## Outcome

Did **not** clear Round 1. Posting this anyway — a failed attempt with honest notes is worth more to the next person than a selected candidate's vague "prepare well bro."

**What I'd do differently:**
- Grind grid-BFS variants until they're muscle memory
- Actually practise reading buggy code, not just writing fresh code
- Rebalance prep time away from DP, toward graphs
- Start contests earlier

---

*If this helped, ⭐ the repo. PRs with more OA experiences are welcome.*
