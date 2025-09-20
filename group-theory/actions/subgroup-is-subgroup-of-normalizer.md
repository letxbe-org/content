---
type: result
title: A subgroup is a subgroup of its own normalizer
---

## Statement

Let $G$ be a [group](@group) and $H \le G$ be a [subgroup](@subgroup). Then $H \le N_G(H)$, where $N_G(H)$ denotes the [normalizer](@normalizer) of $H$.

## Proof

By the [subgroup criterion](@subgroup-criterion), since $H$ is already a subgroup of $G$, we only have to show that $H \subseteq N_G(H)$.

Let $g \in H$ be arbitrary. We then have to show that $g \in N_G(H)$, that is $gHg^{-1} = H$.

First, let $ghg^{-1} \in gHg^{-1}$ for some $h \in H$. Since $H$ is a [group](@group), we have that $ghg^{-1} \in H$. So we conclude $gHg^{-1} \subseteq H$.

Next, let $h \in H$. Then since $H$ is a [group](@group), $g^{-1}hg \in H$. We now have that $$ \begin{aligned} h &= (gg^{-1})h(gg^{-1}) \\ &= g(g^{-1}hg)g^{-1} \\ &\in gHg^{-1}, \end{aligned} $$ so $H \subseteq gHg^{-1}$.

From both inclusions we conclude that $gHg^{-1} = H$. This means that $g \in N_G(H)$. And since $g$ was chosen arbitrarily, we conclude that $H \subseteq N_G(H)$.

QED.
