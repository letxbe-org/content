---
type: result
title: Homomorphisms preserve inverses
---

## Statement

Let $G$ and $H$ be [groups](@group) with identities $1_G$ and $1_H$ respectively, and let $\varphi: G \to H$ be a [homomorphism](@group-homomorphism). Then $\varphi(x^{-1}) = \varphi(x)^{-1}$ for all $x \in G$.

## Proof

Using [@](@homomorphisms-preserve-identity) and the property of homomorphisms, we have that $$\varphi(x^{-1})\varphi(x) = \varphi(x^{-1}x) = \varphi(1_G) = 1_H.$$

So $\varphi(x^{-1})$ is an inverse of $\varphi(x)$. From [@](@inverse-is-unique), we conclude that $\varphi(x^{-1}) = \varphi(x)^{-1}$.

QED.
