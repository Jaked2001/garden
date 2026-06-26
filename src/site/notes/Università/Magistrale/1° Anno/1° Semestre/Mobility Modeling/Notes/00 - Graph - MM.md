---
{"dg-publish":true,"permalink":"/universita/magistrale/1-anno/1-semestre/mobility-modeling/notes/00-graph-mm/","tags":["UNI"],"dg-note-properties":{"aliases":null,"Materia":"MM","Tipo":"T","Stato":"🟠 Studiare","Slide":["[0 - Introduction to graphs - MM.pdf](/img/user/Universit%C3%A0/Magistrale/1%C2%B0%20Anno/1%C2%B0%20Semestre/Mobility%20Modeling/Notes/Allegati/0%20-%20Introduction%20to%20graphs%20-%20MM.pdf)"],"PDF":null,"Parents":["[[📐 Mobility Modeling]]"],"Children":null,"Siblings":null,"tags":["UNI"]}}
---

# [[Università/Magistrale/1° Anno/1° Semestre/Mobility Modeling/Notes/00 - Graph - MM\|00 - Graph - MM]]

Graphs are useful mathematical models for representing urban and transportation networks.

![Schermata 2024-10-10 alle 16.09.44.png](/img/user/Schermata%202024-10-10%20alle%2016.09.44.png)


## Directed graph

```ad-Definizione
title: Directed Graph

A **directed graph** is a set of $N$ nodes and a set of $A$ arcs or links whose elements are ordered pairs of distinct nodes.

It is represented as

$
G = (N, A)
$

```

- Nodes are usually numbered with integers.
- Arcs are either named with integers, or with the pair of nodes they connect

![00 - Graph 2024-10-10 16.12.25.excalidraw.png](/img/user/Excalidraw/Excalidraw-2/00%20-%20Graph%202024-10-10%2016.12.25.excalidraw.png)
[[Excalidraw/Excalidraw-2/00 - Graph 2024-10-10 16.18.33.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Excalidraw-2/00 - Graph 2024-10-10 16.12.25.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Excalidraw-2/Forward star - 00 - Graph 2024-10-24 12.48.02.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Excalidraw-2/00 - Graph 2024-10-10 16.12.25.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Excalidraw-2/Directed path - 00 - Graph 2024-10-24 13.00.21.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Excalidraw-2/00 - Graph 2024-10-10 16.12.25.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Excalidraw-2/Undirected path - 00 - Graph 2024-10-24 13.08.17.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Excalidraw-2/00 - Graph 2024-10-10 16.12.25.excalidraw\|🖋 Edit in Excalidraw]][[Tree vs Path00 - Graph - MM 2024-10-28 15.42.39.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Excalidraw-2/Spanning tree - 00 - Graph - MM 2024-10-28 15.45.05.excalidraw\|🖋 Edit in Excalidraw]][[Excalidraw/Excalidraw-2/Storing and retrieving paths - 00 - Graph - MM 2024-10-30 11.30.32.excalidraw\|🖋 Edit in Excalidraw]]%%

This tree can be stored as an array $p$ of pointers:
$$
\begin{bmatrix}
\text{index} & 1 & 2 & 3 & 4 & 5 & 6 & 7 & 8 \\
p & 0 & 5 & 1 & 2 & 1 & 2 & 4 & 3
\end{bmatrix}
$$



