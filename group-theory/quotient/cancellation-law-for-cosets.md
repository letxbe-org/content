---
type: result
title: Cancellation laws for cosets
---

## Statement

Let $G$ be a [group](@group) and $H \le G$ be a [subgroup](@subgroup). Let $x, y \in G$ be elements. Then $$ xH = yH \iff y^{-1}xH = H, $$ where $xH, yH$ and $y^{-1}xH$ denote [cosets](@coset).

## Proof

First, suppose that $xH = yH$. Since $1 \in H$ by [@](@subgroup-contains-identity), we have that $$ x = x1 \in xH = yH, $$ so that $x = yh$ for some $h \in H$. Left-multiplying with $y^{-1}$ yields $$ y^{-1}x = h \in H. $$ From [@](@any-element-of-coset-represents-it) we obtain $y^{-1}xH = H$.

Next, suppose that $y^{-1}xH = H$. Then since $1 \in H$ by [@](@subgroup-contains-identity), we have that $$ y^{-1}x = y^{-1}x1 \in y^{-1}xH = H, $$ so that $y^{-1}x = h$ for some $h \in H$. Left-multiplying with $y$ yields $$ x = yh \in yH. $$ From [@](@any-element-of-coset-represents-it) we obtain $xH = yH$.

QED.
