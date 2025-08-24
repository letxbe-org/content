---
type: result
title: The kernel of a homomorphism is a normal subgroup
---

## Statement

Let $G$ and $H$ be [groups](@group) and $\varphi: G \to H$ be a [homomorphism](@group-homomorphism). The [kernel](@kernel) of $\varphi$ is a [normal subgroup](@normal-subgroup) of $G$. That is, $$ \text{Kern}(\varphi) \trianglelefteq G.$$

## Proof

From [@](@kernel-is-subgroup) we know that $\text{Kern}(\varphi) \le G$. Let $g \in G, n \in \text{Kern}(\varphi)$. Then $\varphi(n) = 1$.

Using [@](@homomorphisms-preserve-identity) and the property of [homomorphisms](@group-homomorphism), we have that $$\begin{aligned} \varphi(gng^{-1}) &= \varphi(g) \varphi(n) \varphi(g^{-1}) \\ &= \varphi(g) 1 \varphi(g^{-1}) \\ &= \varphi(g) \varphi(g^{-1}) \\ &= \varphi(gg^{-1}) \\ &= \varphi(1) \\ &= 1, \end{aligned}$$ so we conclude that $gng^{-1} \in \text{Kern}(\varphi)$.

QED.
