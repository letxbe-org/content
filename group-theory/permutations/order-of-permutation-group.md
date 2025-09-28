---
type: result
title: Order of permutation group
---

## Statement

Let $n \ge 1$ be an integer. Then the order of the [permutation group](@permutation-group) $S_n$ is $n!$.

## Proof

Let $\sigma \in S_n$. The element $1$ can be send to any of the numbers $1, ..., n$, so there are $n$ choices for $\sigma(1)$. Since $\sigma$ is a bijection, $\sigma(1) \neq \sigma(2)$. So there are $n-1$ choices left for $\sigma(2)$. Then $\sigma(3)$ can be any number except $\sigma(1), \sigma(2)$, which are $n-2$ choices.

Continuing this, we see that there are exactly $n \cdot (n-1) \cdot (n-2) \cdot ... \cdot 2 \cdot 1 = n!$ options for $\sigma$. Thus the set of all permutations $S_n$ contains $n!$ permutations.

QED.
