---
type: result
title: The center is a subgroup
---

## Statement

Let $G$ be a [group](@group). Then the [center](@center) of $G$ is a [subgroup](@subgroup) of $G$, that is $Z(G) \le G$.

## Proof

We will prove this directly from the definition of a [subgroup](@subgroup).

First, note that per [@](@group), we have that $1x = x1 = 1$ for all $x \in G$. So $1 \in Z(G)$. This means that $Z(G) \neq \emptyset$.

Second, let $g, h \in Z(G)$. Then $gx=xg$ and $hx=xh$ for all $x \in G$. We want to show that $gh \in Z(G)$, so $(gh)x = x(gh)$ for all $x \in G$. Let $x \in G$ be arbitrary. Then we have that $$ (gh)x = g(hx) = g(xh) = (gx)h = (xg)h = x(gh) .$$

Third, let $g \in Z(G)$. Then $gx=xg$ for all $x \in G$ We want to show that $g^{-1} \in Z(G)$, that is $g^{-1}x = xg^{-1}$ for all $x \in G$. Let $x \in G$ be arbitrary. Then $gx=xg$. Left- and right-multiplying with $g^{-1}$ yields $xg^{-1} = g^{-1}x$, as required.

QED.
