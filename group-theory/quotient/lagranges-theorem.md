---
type: result
title: Lagrange's Theorem
---

## Statement

Let $G$ be a [finite group](@group) and $H \le G$ be a [subgroup](@subgroup). Then the [order](@order) of $H$ divides the [order](@order) of $G$. More specifically, $$ |G| = [G:H] |H|, $$ where $[G:H]$ denotes the [index](@index) of $G$ in $H$.

## Proof

Since $G$ is finite, the [set of cosets](@set-of-cosets) $G/H$ is also finite. Number the elements of $G/H$ as $g_1H, g_2H, ..., g_nH$ for some $n\in\N$.

Since $G/H$ is a [partition](@cosets-partition-group) of $G$, we have that: $$ |G| = |g_1H| + |g_2H| + ... + |g_nH| = \sum_{i=1}^n |g_iH| $$

From [@](@order-of-cosets-equals-order-of-subgroup) we obtain that $|g_iH|=|H|$ for all $1 \le i \le n$, so $$ |G| = \sum_{i=1}^n |g_iH| = \sum_{i=1}^n |H| = n|H| $$

And since there are $n$ different cosets, the [index](@index) $[G:H]=n$. So we conclude

$$ |G| = [G:H] |H| $$

QED.
