---
type: result
title: Quotient group is group
---

## Statement

Let $G$ be a [group](@group) and $N \trianglelefteq G$ a [normal subgroup](@normal-subgroup). Then the [quotient group](@quotient-group) $G/N$ with [coset multiplication](@quotient-group) is a [group](@group).

## Proof

From [@](@coset-multiplication-is-well-defined-for-normal-subgroups) it follows that coset-multiplication is a well-defined [binary operation](@binary-operation).

### Associativity

Let $a,b,c \in G$. Since the operation on $G$ is [associative](@group), we have that $$\begin{aligned} aN * (bN * cN) &= aN * (bc)N \\ &= (a(bc))N \\ &= ((ab)c)N \\ &= (ab)N * cN \\ &= (aN * bN) * cN, \end{aligned}$$ so we conclude that coset multiplication is associative.

### Identity

Let $a \in G$. Since $G$ has [identity](@group) $1$, we have that $$aN * 1N = (a1)N = aN = (1a)N = 1N * aN,$$ so we conclude that $G/N$ has identity $1N$.

### Inverses

Let $a \in G$. Since $G$ has [inverses](@group), we have that $a^{-1} \in G$. Now we see that $$aN * a^{-1}N = (aa^{-1})N = 1N = (a^{-1}a)N = a^{-1}N * aN,$$ so we conclude that $a^{-1}N$ is the inverse of $aN$.

QED.
