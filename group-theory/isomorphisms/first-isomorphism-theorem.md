---
type: result
title: First Isomorphism Theorem
---

## Statement

Let $G, H$ be [groups](@group) and $\varphi: G \to H$ be a [homomorphism](@group-homomorphism). Then the [quotient](@quotient-group) of $G$ by the [kernel](@kernel) of $\varphi$ is [isomorphic](@group-isomorphism) to the image of $\varphi$. That is,

$$ G / \text{Kern}(\varphi) \cong \text{Im}(\varphi). $$

## Proof

Define $K := \text{Kern}(\varphi)$. Consider the function $\psi: G / K \to \text{Im}(\varphi)$, given by $\psi(gK) = \varphi(g)$. We will prove that this function is an [isomorphism](@group-isomorphism).

First, we will show that $\psi$ is a homomorphism. Let $gK, hK \in G/K$. Using [coset multiplication](@quotient-group) and the fact that $\varphi$ is a homomorphism, we then have that

$$ \begin{aligned} \psi(gK * hK) &= \psi((gh)K) \\ &= \varphi(gh) \\ &= \varphi(g)\varphi(h) \\ &= \psi(gK) \psi(hK), \end{aligned} $$

which shows that $\psi$ is a [homomorphism](@group-homomorphism).

Next, we will show that $\psi$ is injective. Suppose that $xK \in \text{Kern}(\psi)$ for some $x \in G$. Then $\psi(xK) = 1$. We then have $\varphi(x) = 1$, so that $x \in K$. Using [@](@any-element-of-coset-represents-it), we have that $xK = K$, the [identity](@group) in $G/K$. This means that $\text{Kern}(\psi) = \{K\}$. From [@](@homomorphism-injective-iff-trivial-kernel), we conclude that $\psi$ is injective.

Finally, we prove that $\psi$ is surjective. Let $y \in \text{Im}(\varphi)$. Then there exists some $g \in G$ such that $\varphi(g) = y$. Choose $x := gK$. Then $$ \psi(x) = \psi(gK) = \varphi(g) = y,$$ which shows that $\psi$ is surjective.

Since $\psi$ is a homomorphism, injection and surjection, we conclude that $\psi$ is an isomorphism. Thus $G/\text{Kern}(\varphi) \cong \text{Im}(\varphi)$.

QED.
