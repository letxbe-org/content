---
type: result
title: Homomorphisms preserve powers
---

## Statement

Let $G$ and $H$ be [groups](@group) and $\varphi: G \to H$ be a [homomorphism](@group-homomorphism). Then $\varphi(x^n) = \varphi(x)^n$ for all $x \in G$ and $n \in \Z$.

## Proof

First, we will prove the statement for $n \in \N$ using induction on $n$. The base case $n=0$ follows from [@](@power) and [@](@homomorphisms-preserve-identity).

Now, suppose that $\varphi(x^k) = \varphi(x)^k$ for some $k \in \N$. Then, using the property of homomorphisms, we have $$\begin{aligned} \varphi(x^{k+1}) &= \varphi(x^kx) \\ &= \varphi(x^k)\varphi(x) \\ &= \varphi(x)^k \varphi(x) \\ &= \varphi(x)^{k+1}, \end{aligned}$$ which concludes the induction.

Next, we will prove the statement for non-positive integers using induction on $n$. The base case $n=0$ follows from [@](@power) and [@](@homomorphisms-preserve-identity).

Now, suppose that $\varphi(x^{-k}) = \varphi(x)^{-k}$ for some $k\in\N$. Then, using the property of homomorphisms and [@](@homomorphisms-preserve-inverses), we have that $$\begin{aligned} \varphi(x^{-(k+1)}) &= \varphi(x^{-k-1}) \\ &= \varphi(x^{-k}x^{-1}) \\ &= \varphi(x^{-k}) \varphi(x^{-1}) \\ &= \varphi(x)^{-k} \varphi(x)^{-1} \\ &= \varphi(x)^{-k-1} \\ &= \varphi(x)^{-(k+1)}, \end{aligned}$$ which concludes the induction.

QED.
