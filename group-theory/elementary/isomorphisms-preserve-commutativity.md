---
type: result
title: Isomorphisms preserve commutativity
---

## Statement

Let $G$ and $H$ be [isomorphic](@group-isomorphism) [groups](@group), that is $G \cong H$. Then $G$ is [commutative](@group) if and only if $H$ is [commutative](@group).

## Proof

Let $\varphi: G \to H$ be an [isomorphism](@group-isomorphism).

First, suppose that $G$ is commutative. Let $h_1, h_2 \in H$. Since $\varphi$ is a bijection, there exist $g_1, g_2 \in G$ such that $\varphi(g_1) = h_1$ and $\varphi(g_2) = h_2$. We now have that $$\begin{aligned} h_1h_2 &= \varphi(g_1)\varphi(g_2) \\ &= \varphi(g_1g_2) \\ &= \varphi(g_2g_1) \\ &= \varphi(g_2)\varphi(g_1) \\ &= h_2h_1, \end{aligned}$$ from which we conclude that $H$ is also commutative.

Next, suppose that $H$ is commutative. Let $g_1, g_2 \in G$ and let $h_1 := \varphi(g_1), h_2 := \varphi(g_2)$. Then $$\begin{aligned} \varphi(g_1g_2) &= \varphi(g_1)\varphi(g_2) \\ &= h_1h_2 \\ &= h_2h_1 \\ &= \varphi(g_2)\varphi(g_1) \\ &= \varphi(g_2g_1). \end{aligned}$$

And since $\varphi$ is a bijection, we can conclude that $g_1g_2 = g_2g_1$. That is, $G$ is commutative.

QED.
