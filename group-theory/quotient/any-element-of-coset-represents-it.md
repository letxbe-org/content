---
type: result
title: Any element of a coset represents it
---

## Statement

Let $G$ be a [group](@group) and $H \le G$ be a [subgroup](@subgroup). If some $a \in G$ is in the [coset](@coset) $bH$ for some $b \in G$, then the [cosets](@coset) $aH$ and $bH$ are equal. That is, $$a \in bH \implies aH = bH \quad \text{ for } a,b \in G.$$

## Proof

Suppose that $a \in bH$ for some $a,b \in G$. Then $a = bh$ for some $h \in H$. So $b = ah^{-1}$.

First, suppose that $ah_1 \in aH$ for some $h_1 \in H$. Since $H$ is a [subgroup](@subgroup), $hh_1 \in H$. Now we have that $ah_1 = bhh_1 \in bH$, so $aH \subseteq bH$.

Next, suppose that $bh_2 \in bH$ for some $h_2 \in H$. Since $H$ is a [subgroup](@subgroup), $h^{-1}h_2 \in H$. Now we have that $bh_2 = ah^{-1}h_2 \in aH$, so $bH \subseteq aH$.

From both inclusions we conclude that $aH = bH$.

QED.
