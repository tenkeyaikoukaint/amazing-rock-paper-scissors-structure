

# Rock-Paper-Scissors Amazing Structure: Calculate is Division(Introduction)

## Abstract

This paper introduces a novel algebraic formulation of the Rock-Paper-Scissors (RPS) dynamic. While traditionally modeled as a simple cyclic group $C_3$ where elements are directly mapped to a zero-sum outcome, we demonstrate that the interaction between elements is fundamentally a **division operation**. By redefining the engagement of two elements as $x \cdot y^{-1}$, we unveil a three-layered algebraic structure consisting of objects (hands), operations (division), and states (phase shifts). This elegantly simple paradigm provides a robust framework for procedural generation, algorithmic evaluation, and non-associative topological modeling.

## 1. Introduction: The Tripartite Structure

The core of this structure lies in abandoning the conventional comparative logic (e.g., if $A > B$ then win). Instead, we posit that **calculate is division**.

Let the set of elements (hands) be defined as:


$$H = \{Rock, Scissors, Paper\}$$

Let the set of state shifts (outcomes) be defined as:


$$O = \{id, ++, --\}$$


where $id$ represents a tie (identity), $++$ represents a forward phase shift (win first), and $--$ represents a backward phase shift (win second).

## 2. Formal Definition

For any two elements $x, y \in H$, the relational outcome is derived by multiplying $x$ by the inverse of $y$. The foundational axioms are defined as follows:

**Identity (Tie):**


$$Rock \cdot Rock^{-1} = id$$

$$Scissors \cdot Scissors^{-1} = id$$

$$Paper \cdot Paper^{-1} = id$$

**Forward Phase (Win First):**


$$Rock \cdot Scissors^{-1} = ++$$

$$Scissors \cdot Paper^{-1} = ++$$

$$Paper \cdot Rock^{-1} = ++$$

**Backward Phase (Win Second):**


$$Rock \cdot Paper^{-1} = --$$

$$Scissors \cdot Rock^{-1} = --$$

$$Paper \cdot Scissors^{-1} = --$$

## 3. The Relational Matrix

This division operation yields a perfectly symmetric interaction matrix, mapping the absolute elements of $H$ into the relative states of $O$.

| Numerator ($x$) \ Denominator ($y^{-1}$) | $Rock^{-1}$ | $Scissors^{-1}$ | $Paper^{-1}$ |
| --- | --- | --- | --- |
| **$Rock$** | $id$ | $++$ | $--$ |
| **$Scissors$** | $--$ | $id$ | $++$ |
| **$Paper$** | $++$ | $--$ | $id$ |

This mathematical simplicity proves that RPS is not merely a game of cyclic dominance, but a rigorous algebraic system driven by inverse relations.

