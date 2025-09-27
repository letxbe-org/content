---
type: result
title: The stabilizer is a subgroup
---

## Statement

Let $G$ be a [group](@group) [acting](@group-action) on a set $X$ and let $x \in X$ be an element. Then the [stabilizer](@stabilizer) of $x$ is a subgroup of $G$, that is $$ \text{Stab}(x) \le G. $$

## Proof

We will use the [subgroup criterion](@subgroup-criterion).

First, note that $1 \cdot x = x$, so that $1 \in \text{Stab}(x)$. This means that $\text{Stab}(x) \neq \emptyset$.

Next, let $g,h \in \text{Stab}(x)$ be arbitrary. Then $g \cdot x = x$ and $h \cdot x = x$. By the [cancellation law for group actions](@cancellation-law-for-group-actions), we obtain $h^{-1} \cdot x = x$.

We now have that $$ (gh^{-1}) \cdot x = g \cdot (h^{-1} \cdot x) = g \cdot x = x, $$ so that $gh^{-1} \in \text{Stab}(x)$. This proves that $\text{Stab}(x)$ is a subgroup of $G$.

QED.
