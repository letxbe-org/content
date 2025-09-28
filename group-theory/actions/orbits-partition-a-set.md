---
type: result
title: Orbits partition a set
---

## Statement

Let $G$ be a [group](@group) and $\cdot$ be a [group action](@group-action) on a set $X$. Then the set [orbits](@orbit) $\{ \text{Orb}(x) : x \in X \}$ is a partition of $X$.

## Proof

Define $O := \{ \text{Orb}(x) : x \in X \}$ to be the set of all [orbits](@orbit). We will show that $\emptyset \notin O$, $\cup_{x \in X} \text{Orb}(x) = X$ and $\text{Orb}(x) \cap \text{Orb}(y) \neq \emptyset \implies \text{Orb}(x) = \text{Orb}(y)$ for all $x,y \in X$.

First, let $\text{Orb}(x) \in O$ be an orbit for some $x \in X$. Since $1 \in G$ per definition of a [group](@group), we have that $x = 1 \cdot x \in \text{Orb}(x)$ using the definition of [group actions](@group-action). So $\text{Orb}(x) \neq \emptyset$, thus $\emptyset \notin O$.

Next, since $\text{Orb}(x) \subseteq X$ for all $x \in X$, it is clear that $\cup_{x \in X} \text{Orb}(x) \subseteq X$. Let $x \in X$ be arbitrary. Since $1 \in G$ per definition of a [group](@group), we have that $x = 1 \cdot x \in \text{Orb}(x)$ using the definition of [group actions](@group-action). So $x \in \cup_{x \in X} \text{Orb}(x)$. This shows that $X \subseteq \cup_{x \in X} \text{Orb}(x)$. From both we inclusions we conclude that $\cup_{x \in X} \text{Orb}(x) = X$.

Finally, suppose that $\text{Orb}(x), \text{Orb}(y) \in O$ for some $x,y \in X$ such that $\text{Orb}(x) \cap \text{Orb}(y) \neq \emptyset$. Then there exists some $z \in X$ such that $z \in \text{Orb}(x)$ and $z \in \text{Orb}(y)$. This means that $z = g_1 \cdot x = g_2 \cdot y$ for some $g_1, g_2 \in G$. By the [cancellation law for group actions](@cancellation-law-for-group-actions), we have that $x = (g_1^{-1}g_2) \cdot y$.

Let $a \in \text{Orb}(x)$ be arbitrary. Then $a = g \cdot x$ for some $g \in G$. Define $g' := gg_1^{-1}g_2$, then $g' \in G$. We then have that $$ g' \cdot y = (gg_1^{-1}g_2) \cdot y= g \cdot ((g_1^{-1}g_2) \cdot y) = g \cdot x = a \in \text{Orb}(y),$$ so that $\text{Orb}(x) \subseteq \text{Orb}(y)$. Similarly we obtain $\text{Orb}(y) \subseteq \text{Orb}(x)$, so that $\text{Orb}(x) = \text{Orb}(y)$.

QED.
