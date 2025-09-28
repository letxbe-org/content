---
type: result
title: The permutation group is a group
---

## Statement

Let $n \ge 1$ be an integer. Then the [permutation group](@permutation-group) $S_n$ is a [group](@group).

## Proof

We will prove the three properties of a group.

The [binary operation](@binary-operation) used in the permutation group is _function composition_ $\circ$. We will prove that it is [associative](@binary-operation). Let $\sigma, \tau, \pi \in S_n$ be arbitrary. Let $k \in \{1,...,n\}$. Then $$ \begin{aligned} (\sigma \circ (\tau \circ \pi))(k) &= \sigma((\tau \circ \pi)(k)) \\ &= \sigma(\tau(\pi(k))) \\ &= (\sigma \circ \tau)(\pi(k)) \\ &= ((\sigma \circ \tau) \circ \pi)(k) .\end{aligned} $$ Since this holds for all $k \in \{1,...,n\}$, we have that $\sigma \circ (\tau \circ \pi) = (\sigma \circ \tau) \circ \pi$ for all $\sigma, \tau, \pi \in S_n$. That is, function composition $\circ$ is associative.

Consider the function $\text{id}: \{1,...,n\} \to \{1,...,n\}$, given by $\text{id}(k) = k$. This function is a permutation of $\{1,...,n\}$, so $\text{id} \in S_n$. Note that $\sigma \circ \text{id} = \text{id} \circ \sigma = \sigma$ for all $\sigma \in S_n$, so that $\text{id}$ is the identity for $S_n$.

Finally, we will show that inverses exist. Let $\sigma \in S_n$ be arbitrary. Since $\sigma$ is a bijection, it has a two-sided inverse $\sigma^{-1} \in S_n$ such that $\sigma \circ \sigma^{-1} = \sigma^{-1} \circ \sigma = \text{id}$.

Since all properties of a group are satisfied, we conclude that $S_n$ is a group.

QED.
