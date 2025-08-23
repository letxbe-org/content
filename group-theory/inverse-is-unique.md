---
type: result
title: The inverse of a group element is unique
---

## Statement

Let $G$ be a [group](@group) and $a \in G$ some element. Then $a^{-1}$, the inverse of $a$, is unique.

## Proof

Suppose that $b$ and $c$ are both inverses of $a$. Then by property 3 of a [group](@group), we have that $a*b=1$ and $c*a=1$. This gives $$\begin{aligned} c &= c * 1 \\ &= c * (a * b) \\ &= (c * a) * b \\ &= 1 * b \\ &= b. \end{aligned}$$ Thus the inverse is unique.

QED.
