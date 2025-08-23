---
type: result
title: The image of a homomorphism is a subgroup
---

## Statement

Let $G$ and $H$ be [groups](@group) and $\varphi: G \to H$ be a [homomorphism](@group-homomorphism). The image of $\varphi$ is a [subgroup](@subgroup) of $H$. That is, $$ \text{Im}(\varphi) \le H.$$

## Proof

Using [@](@homomorphisms-preserve-identity), we have that $\varphi(1) = 1$, so that $1 \in \text{Im}(\varphi)$. That is, $\text{Im}(\varphi) \neq \emptyset$.

Let $x,y \in \text{Im}(\varphi)$. Then there exist $a,b \in G$ such that $\varphi(a) = x$ and $\varphi(b) = y$. This means that also $b^{-1} \in G$, and thus $ab^{-1} \in G$. Using the property of [homomorphisms](@group-homomorphism) and [@](@homomorphisms-preserve-powers), we have that $$ \begin{aligned} \varphi(ab^{-1}) &= \varphi(a) \varphi(b^{-1}) \\ &= \varphi(a) \varphi(b)^{-1} \\ &= xy^{-1}. \end{aligned} $$ So $xy^{-1} \in \text{Im}(\varphi)$.

Applying the [subgroup criterion](@subgroup-criterion), we conclude that $\text{Im}(\varphi) \le H$.

QED.
