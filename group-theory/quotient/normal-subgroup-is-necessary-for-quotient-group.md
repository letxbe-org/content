---
type: result
title: Normal subgroup is necessary for quotient group
---

## Statement

Let $G$ be a [group](@group) and $N \le G$ a [subgroup](@subgroup). If the [coset multiplication](@quotient-group) on the [set of cosets](@set-of-cosets) $G/N$ is well-defined, then $N$ must be a [normal subgroup](@normal-subgroup).

## Proof

Suppose that [coset multiplication](@quotient-group) is well-defined. Then for any two coset representatives, the product will remain the same. That is, for all $x,x',y,y' \in G$, if $xN = x'N$ and $yN = y'N$, then $(xy)N = (x'y')N$.

Let $g \in G$ and $n \in N$ be arbitrary. Choose $x=1$, $x'=n$ and $y=y'=g^{-1}$. Then we have that $$g^{-1}N = (ng^{-1})N.$$

We will show that $N = (gng^{-1})N$. Let $a \in N$ be arbitrary. Then $g^{-1}a \in g^{-1}N = (ng^{-1})N$. So $g^{-1}a=ng^{-1}b$ for some $b \in N$. This means that $a = gng^{-1}b \in (gng^{-1})N$. So $N \subseteq (gng^{-1})N$.

Now let $gng^{-1}c \in (gng^{-1})N$ be arbitrary for some $c \in N$. Then $ng^{-1}c \in (ng^{-1})N = g^{-1}N$. So $ng^{-1}c = g^{-1}d$ for some $d \in N$. This means that $gng^{-1}c = d \in N$. So $(gng^{-1})N \subseteq N$. From both inclusions we conclude that $N = (gng^{-1})N$.

Since $N$ [contains the identity](@subgroup-contains-identity) $1$, we have that $gng^{-1} = gng^{-1}1 \in (gng^{-1})N = N$, which proves that $N$ is a [normal subgroup](@normal-subgroup).

QED.
