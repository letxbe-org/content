---
type: result
title: Isomorphisms preserve order
---

## Statement

Let $G$ and $H$ be [isomorphic](@group-isomorphism) [groups](@group), that is $G \cong H$. Then the [order](@order) is preserved, that is $|x| = |\varphi(x)|$ for all $x \in G$.

## Proof

Let $\varphi: G \to H$ be an [isomorphism](@group-isomorphism) and let $x \in G$.

First, suppose that the [order](@order) of $x$ is finite, that is $|x| = n$ for some $n \in \Z^+$. Then $x^n = 1$. Using [@](@homomorphisms-preserve-powers) and [@](@homomorphisms-preserve-identity), we have that $\varphi(x)^n = \varphi(x^n) = \varphi(1) = 1$.

By contradiction, suppose there exists some $m \in \Z^+$ such that $m<n$ and $\varphi(x)^m = 1$. Then using [@](@homomorphisms-preserve-powers) and [@](@homomorphisms-preserve-identity), we have that $\varphi(x^m) = 1 = \varphi(1)$. And since $\varphi$ is a bijection, we get $x^m = 1$.

But since $n$ is the _smallest_ such integer, we conclude that a smaller integer $m$ cannot exist. So this is a contradiction. We conclude that $n$ is the smallest positive integer such that $\varphi(x)^n = 1$. So $|\varphi(x)| = n$.

Next, suppose that the [order](@order) of $x$ is infinite. By contradiction, suppose that there exists some integer $m \in \Z^+$ such that $\varphi(x)^m = 1$. Then using [@](@homomorphisms-preserve-powers) and [@](@homomorphisms-preserve-identity), we have that $\varphi(x^m) = 1 = \varphi(1)$. And since $\varphi$ is a bijection, we get $x^m = 1$. This is a contradiction, so we conclude that such integer $m$ cannot exist. That is, $|\varphi(x)|$ is infinite.
