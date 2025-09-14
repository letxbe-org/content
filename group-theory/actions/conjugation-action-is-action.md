---
type: result
title: The conjugation action is a group action
---

## Statement

Let $G$ be a [group](@group). The [conjugation action](@conjugation-action) is a [group action](@group-action) on $G$.

## Proof

First, let $g_1, g_2, a \in G$ be arbitrary. Using [@](@inverse-of-product), we have that

$$ \begin{aligned} g_1 \cdot (g_2 \cdot a) &= g_1 \cdot (g_2 a g_2^{-1}) \\ &= g_1 g_2 a g_2^{-1} g_1^{-1} \\ &= (g_1g_2)a(g_1g_2)^{-1} \\ &= (g_1g_2) \cdot a. \end{aligned} $$

Next, let $a \in G$ be arbitrary. We have that $$ 1 \cdot a = 1 a 1^{-1} = a. $$

Since all properties are satisfied, we conclude that conjugation is a group action.

QED.
