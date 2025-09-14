---
type: result
title: The order of cosets equals the order of a subgroup
---

## Statement

Let $G$ be a [group](@group) and $H \le G$ be a [subgroup](@subgroup). Then the [order](@order) of the [coset](@coset) $gH$ equals the order of the subgroup $H$.

## Proof

Let $g \in G$. Consider the function $f: H \to gH$, given by $f(h) = gh$. We will show that this function is injective and surjective.

First, suppose that $f(h_1) = f(h_2)$ for some $h_1, h_2 \in H$. Then $gh_1 = gh_2$. By the [cancellation law](@cancellation-law), we obtain that $h_1 = h_2$. We conclude that $f$ is injective.

Next, let $y \in gH$ be arbitrary. Then $y = gh$ for some $h \in H$. Choose $x := h$. Then $$ f(x) = f(h) = gh = y, $$ so $f$ is surjective.

Since $f$ is both injective and surjective, $f$ is a bijection. So $|gH| = |H|$.

QED.
