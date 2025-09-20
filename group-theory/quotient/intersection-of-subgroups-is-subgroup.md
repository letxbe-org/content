---
type: result
title: The intersection of two subgroups is a subgroup
---

## Statement

Let $G$ be a [group](@group) and $H,K \le G$ be [subgroups](@subgroup). Then the intersection $H \cap K \le G$.

## Proof

We will use the [subgroup criterion](@subgroup-criterion).

First, using [@](@subgroup-contains-identity), we have that $1 \in H$ and $1 \in K$. So $1 \in H \cap K$. That is, $H \cap K \neq \emptyset$.

Next, let $x, y \in H \cap K$. Then $x,y \in H$ and $x,y \in K$. Again uing the [subgroup criterion](@subgroup-criterion), we have that $xy^{-1} \in H$ and $xy^{-1} \in K$. So $xy^{-1} \in H \cap K$.

QED.
