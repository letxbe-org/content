---
type: result
title: Cancellation law for group actions
---

## Statement

Let $G$ be a [group](@group) and $\cdot$ be a [group action](@group-action) on a set $X$. Let $g, h \in G$ and $x \in X$. Then $$ g \cdot x = h \cdot x \iff (h^{-1}g) \cdot x = x. $$

## Proof

First, suppose that $g \cdot x = h \cdot x$. Applying $h^{-1}$ to both sides, we get $h^{-1} \cdot (g \cdot x) = h^{-1} \cdot (h \cdot x)$. Using the definition of a [group action](@group-action), we obtain $(h^{-1}g) \cdot x = (h^{-1}h) \cdot x = 1 \cdot x = x$.

Next, suppose that $(h^{-1}g) \cdot x = x$. Applying $h$ to both sides, we get $h \cdot ((h^{-1}g) \cdot x) = h \cdot x$. Using the definition of a [group action](@group-action), we obtain $(hh^{-1}g) \cdot x = h \cdot x$, so that $g \cdot x = h \cdot x$.

QED.
