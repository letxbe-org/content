---
type: result
title: Cancellation law
---

## Statement

Let $G$ be a [group](@group) and $a \in G$ an element.

1. If $ax=ay$ for some $x,y \in G$, then $x=y$.
2. If $xa=ya$ for some $x,y \in G$, then $x=y$.

## Proof

First, suppose that $ax=ay$ for some $x,y \in G$. Left-multipliy both sides by $a^{-1}$, giving $a^{-1}ax = a^{-1}ay$. Simplifying using the [group properties](@group) yields $x=y$.

Next, suppose that $xa=ya$ for some $x,y \in G$. Right-multipliy both sides by $a^{-1}$, giving $xaa^{-1} = yaa^{-1}$. Simplifying using the [group properties](@group) yields $x=y$.

QED.
