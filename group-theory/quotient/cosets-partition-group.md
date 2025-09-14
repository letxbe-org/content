---
type: result
title: Cosets partition a group
---

## Statement

Let $G$ be a [group](@group) and $H \le G$ be a [subgroup](@subgroup). Then the [set of cosets](@set-of-cosets) $G/H$ forms a partition of $G$.

## Proof

First, we will showt that $G/H$ does not contain the empty set $\emptyset$. Let $xH \in G/H$ for some $x \in G$. Since $1 \in H$ by [@](@subgroup-contains-identity), we have that $x = x1 \in xH$, so that $xH \neq \emptyset$. Since $xH$ was chosen arbitrarily, we conclude that $\emptyset \notin G/H$.

Next, we will show that the union of all cosets equals the set $G$. Suppose that $x \in G$. Consider the coset $xH \in G/H$. Since $1 \in H$ by [@](@subgroup-contains-identity), we have that $x = x1 \in xH$. So $x \in \bigcup_{g \in G} gH$.

Suppose now that $x \in \bigcup_{g \in G} gH$. Then $x \in gH$ for some $g \in G$. So $x = gh$ for some $h \in H$. By definition of a [group](@group), we have that $x \in G$.

From both inclusions we conclude that $G = \bigcup_{g \in G} gH$.

Finally, suppose that $xH, yH \in G/H$ such that $xH \cap yH \neq \emptyset$. Then there exists some $z \in xH \cap yH$. From [@](@any-element-of-coset-represents-it), we have that $zH = xH$ and $zH = yH$, which implies that $xH = yH$.

Since we have proven all properties, we conclude that $G/H$ is a partition of $G$.

QED.
