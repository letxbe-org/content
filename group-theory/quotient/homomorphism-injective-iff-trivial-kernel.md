---
type: result
title: A homomorphism is injective if and only if it has a trivial kernel
---

## Statement

Let $G, H$ be [groups](@group) and $\varphi: G \to H$ be a [homomorphism](@group-homomorphism). Then $\varphi$ is injective if and only if the [kernel](@kernel) $\text{Kern}(\varphi) = \{1\}$.

## Proof

First, suppose that $\varphi$ is injective. Let $x \in \text{Kern}(\varphi)$ be arbitrary. Then $\varphi(x) = 1$. Using [@](@homomorphisms-preserve-identity), we have that $\varphi(x) = \varphi(1)$. And since $\varphi$ is injective, we see that $x=1$. So $\text{Kern}(\varphi) \subseteq \{1\}$. Again using [@](@homomorphisms-preserve-identity), we have that $\varphi(1) = 1$, so that $1 \in \text{Kern}(\varphi)$. We conclude that $\text{Kern}(\varphi) = \{1\}$.

Next, suppose that $\text{Kern}(\varphi) = \{1\}$. Let $x,y \in G$ be arbitrary such that $\varphi(x) = \varphi(y)$. Then $\varphi(x) \varphi(y)^{-1} = 1$. Using [@](@homomorphisms-preserve-powers), we have that $\varphi(x) \varphi(y^{-1}) = 1$. And using properties of homomorphisms, we have that $\varphi(xy^{-1}) = 1$.

We see that $xy^{-1} \in \text{Kern}(\varphi)$, so $xy^{-1} = 1$. We conclude that $x=y$, so that $\varphi$ is injective.

QED.
