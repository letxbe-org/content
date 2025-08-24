---
type: result
title: Coset multiplication is well-defined for normal subgroups
---

## Statement

Let $G$ be a [group](@group) and $N \trianglelefteq G$ a [normal subgroup](@normal-subgroup). Then [coset multiplication](@quotient-group) $aN * bN = (ab)N$ is well-defined.

## Proof

To show that the multiplication is well-defined, we have to show that for any two coset representatives, the product will remain the same. So suppose that $aN=a'N$ and $bN = b'N$ for some $a,a',b,b' \in G$. We will show that $aN * bN = a'N * b'N$.

By [@](@subgroup-contains-identity) we have that $1 \in N$. So $a = a1 \in aN = a'N$. This means that $a = a'n_1$ for some $n_1 \in N$. Similarly, $b = b1 \in bN = b'N$, so $b=b'n_2$ for some $n_2 \in N$.

Define $n_3 := b'^{-1}n_1b'$ and $n_4 := n_3n_2$. Then using [@](@inverse-of-inverse-is-original), we see that $n_3 = (b'^{-1})n_1(b'^{-1})^{-1}$, so per definition of a [normal subgroup](@normal-subgroup) we have that $n_3 \in N$. Similarly, we have $n_4 \in N$.

Now we see that $$\begin{aligned} ab &= a'n_1b'n_2 \\ &= a'(b'b'^{-1})n_1b'n_2 \\ &= a'b'(b'^{-1}n_1b')n_2 \\ &= a'b'n_3n_2 \\ &= a'b'n_4 \\ &\in (a'b')N. \end{aligned}$$

From [@](@any-element-of-coset-represents-it) we conclude that $(ab)N = (a'b')N$. That is, $aN * bN = a'N * b'N$.

QED.
