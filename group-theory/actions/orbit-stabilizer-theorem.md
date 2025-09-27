---
type: result
title: Orbit Stabilizer Theorem
---

## Statement

Let $G$ be a [finite group](@group) and $\cdot$ be a [group action](@group-action) on a set $X$. Let $x \in X$ be an element. Then the order of $G$ equals the order of the [orbit](@orbit) of $x$ multiplied by the order of the [stabilizer](@stabilizer) of $x$. That is,

$$ |G| = |\text{Orb}(x)||\text{Stab}(x)| .$$

## Proof

Since $\text{Stab}(x) \le G$ ([@](@stabilizer-is-subgroup)), we can consider the [set of cosets](@set-of-cosets) $G/\text{Stab}(x)$. Now define the function $\varphi: G / \text{Stab}(x) \to \text{Orb}(x)$ given by $\varphi(g\text{Stab}(x)) = g \cdot x$. We will show that this function is well-defined, injective and surjective.

We will first prove that $\varphi$ is well-defined. Suppose that $g\text{Stab}(x) = h\text{Stab}(x)$ for some $g,h \in G$. By the [cancellation law for cosets](@cancellation-law-for-cosets), we have that $h^{-1}g\text{Stab}(x) = \text{Stab}(x)$. And since $1 \in \text{Stab}(x)$ by [@](@subgroup-contains-identity), we have $$ h^{-1}g = h^{-1}g1 \in h^{-1}g\text{Stab}(x) = \text{Stab}(x), $$ so that $(h^{-1}g) \cdot x = x$. Using the [cancellation law for group actions](@cancellation-law-for-group-actions), we obtain $g \cdot x = h \cdot x$. That is, $\varphi(g\text{Stab}(x)) = \varphi(h\text{Stab}(x))$. This shows that $\varphi$ is well-defined.

Next, we will show that $\varphi$ is injective. Suppose that $\varphi(g) = \varphi(h)$ for some $g,h \in G$. Then $g \cdot x = h \cdot x$, so $(h^{-1}g) \cdot x = x$ using [@](@cancellation-law-for-group-actions). This means that $h^{-1}g \in \text{Stab}(x)$. By [@](@any-element-of-coset-represents-it) we have $h^{-1}g\text{Stab} = \text{Stab}(x)$. And by [@](@cancellation-law-for-cosets), we have $g\text{Stab}(x) = h\text{Stab}(x)$, which shows that $\varphi$ is injective.

Finally, we will show that $\varphi$ is surjective. Suppose that $y := g \cdot x \in \text{Orb}(x)$ for some $g \in G$. Consider $z := g\text{Stab}(x) \in G / \text{Stab}(x)$. We then have that $$ \varphi(z) = \varphi(g\text{Stab}(x)) = g \cdot x = y, $$ which shows that $\varphi$ is surjective.

We now have proven that $\varphi$ is a well-defined bijection. This means that $|\text{Orb}(x)| = |G/\text{Stab}(x)|$. By [Langrange's Theorem](@lagranges-theorem), we have that $|G/\text{Stab}(x)| = |G| / |\text{Stab}(x)|$, so that $$ |G| = |\text{Orb}(x)||\text{Stab}(x)|. $$

QED.
