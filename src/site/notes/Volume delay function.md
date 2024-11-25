---
{"dg-publish":true,"permalink":"/volume-delay-function/"}
---

# [[Volume delay function\|Volume delay function]]

In a [[Università/Magistrale/1° Anno/Mobility Modeling/Notes/02 - Traffic Assignment Problem - MM\|Traffic Assignment Problem]], a volume delay function is a function that gives the cost for a user to use a link of a network, taking into account the congestion of the link when that user arrives.

Given a flow on a link equal to $x$, the volume delay function is:
$$
s(x) = f(x)
$$
and it's equal to the cost of $x$ users to use the link.

![Volume delay function 2024-11-24 12.01.46.excalidraw.png](/img/user/Allegati/Volume%20delay%20function%202024-11-24%2012.01.46.excalidraw.png)


Each user $x_{i}$ that enters the link experiences a new cost $s(x_{i})$. The cumulative cost experienced by all users would be:
$$
s(x_{1}) + s(x_{2}) + \cdots + s(x_{n})
$$
If we assume there are enough users that we can consider $x$ to be a continuous variable, $x \in \mathbb{R}$, then, the total cumulative cost, with a flow $x$ in the link, would be:
$$
\int_{0}^{x} s(t) \,{\rm d} t
$$
