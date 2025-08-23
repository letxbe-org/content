---
type: result
title: The kernel of a homomorphism is a subgroup
---

## Statement

Let $G$ and $H$ be [groups](@group) and $\varphi: G \to H$ be a [homomorphism](@group-homomorphism). The [kernel](@kernel) of $\varphi$ is a [subgroup](@subgroup) of $G$. That is, $$ \text{Kern}(\varphi) \le G.$$

## Proof

Using [@](@homomorphisms-preserve-identity), we have that $\varphi(1) = 1$, so that $1 \in \text{Kern}(G)$. That is, $\text{Kern}(G) \neq \emptyset$.

Let $x,y \in \text{Kern}(\varphi)$. Then $\varphi(x) = \varphi(y) = 1$. Using [@](@homomorphisms-preserve-powers), we have that $\varphi(y^{-1}) = \varphi(y)^{-1} = 1^{-1} = 1$. Now using the property of [homomorphisms](@group-homomorphism), we have that $\varphi(xy^{-1}) = \varphi(x) \varphi(y^{-1}) = 1 \cdot 1 = 1$. That is, $xy^{-1} \in \text{Kern}(\varphi)$.

Applying the [subgroup criterion](@subgroup-criterion), we conclude that $\text{Kern}(\varphi) \le G$.

QED.
