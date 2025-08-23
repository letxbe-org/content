---
type: result
title: Subgroup criterion
---

## Statement

Let $G$ be a [group](@group) and $H \subseteq G$ be a subset. Then $H$ is a [subgroup](@subgroup) of $G$ if and only if the following hold:

1. $H \neq \emptyset$.
2. For all $x, y \in H$, $xy^{-1} \in H$.

## Proof

First, suppose that $H$ is a [subgroup](@subgroup) of $G$. Then per definition, $H \neq \emptyset$. Let $x,y \in H$. Per definition, $y^{-1} \in H$ and thus also per definition $xy^{-1} \in H$. So both properties are fulfilled.

Next, suppose that $H \neq \emptyset$ and $\forall x,y \in H: xy^{-1} \in H$. Since $H$ is non-empty, let $a \in H$ be arbitrary. Taking $x=y=a$, we have by property 2 that $xy^{-1} = aa^{-1} = 1 \in H$.

Now let $a \in H$ be arbitrary. Then by choosing $x=1$ and $y=a$, we have $xy^{-1} = 1a^{-1} = a^{-1} \in H$. That is, property 3 of a [subgroup](@subgroup) is fulfilled. Finally, let $a,b \in H$ be arbitrary. Since $b^{-1} \in H$, using property 2 and [@](@inverse-of-inverse-is-original) we have that $a(b^{-1})^{-1} = ab \in H$, fulfilling property 2 of a [subgroup](@subgroup).

Since all properties are fulfilled, we conclude that $H$ is a subgroup of $G$.

QED.
