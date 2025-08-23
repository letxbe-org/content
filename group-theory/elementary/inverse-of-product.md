---
type: result
title: Inverse of a product
---

## Statement

Let $G$ be a [group](@group) and $a,b \in G$. Then $(ab)^{-1} = b^{-1} a^{-1}$.

## Proof

Using the properties of a [group](@group), we have that $$\begin{aligned} (ab)(b^{-1}a^{-1}) &= a(b(b^{-1}a^{-1})) \\ &= a((bb^{-1})a^{-1}) \\ &= a(1a^{-1}) \\ &= aa^{-1} \\ &= 1, \end{aligned}$$ so that $b^{-1}a^{-1}$ is an inverse of $ab$. By [@](@inverse-is-unique), we have that $(ab)^{-1} = b^{-1} a^{-1}$.

QED.
