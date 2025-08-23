---
type: result
title: Homomorphisms preserve identity
---

## Statement

Let $G$ and $H$ be [groups](@group) with identities $1_G$ and $1_H$ respectively and let $\varphi: G \to H$ be a [homomorphism](@group-homomorphism). Then $\varphi(1_G) = 1_H$.

## Proof

Using the property of [homomorphisms](@group-homomorphism) we obtain $$ 1_H \cdot \varphi(1_G) = \varphi(1_G) = \varphi(1_G \cdot 1_G) = \varphi(1_G) \cdot \varphi(1_G).$$

Then, using the [cancellation law](@cancellation-law), we get $1_H = \varphi(1_G)$.

QED.
