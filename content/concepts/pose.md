---
title: 位姿
description:
published: true
date: 2025-05-09T07:06:05.459Z
tags: concept
editor: markdown
dateCreated: 2025-05-09T07:06:05.459Z
---

# 位姿

位姿（Pose）是[位置](/concept/position)（Position）和[姿态](/concept/orientation)（Orientation）的合称。

通常，我们在SE3空间中表示刚体的位姿。几种常见的表达方式有：

1. [刚体变换矩阵](/concept/transform)(Transformation Matrix)：

  $$
  \begin{bmatrix}
   R & t\\
   0 & 1
  \end{bmatrix},
  eg:
  \left[
  	\begin{array}{c|c}
      \begin{matrix}
       1 & 0 & 0\\
       0 & 1 & 0\\
       0 & 0 & 1\\
      \end{matrix}
      & \begin{matrix}
      0.1\\
      0.2\\
      0.3
      \end{matrix} \\
      \hline
      \begin{matrix}
      0 & 0 & 0
      \end{matrix} & 1
    \end{array}
  \right]
  $$

2. 与姿态的组合向量
  a. $[x, y, z, qw, qx, qy, qz]$
  b. $[x, y, z, rx, ry, rz]$

这些表达方式和它的含义一致：通过某种数学语言分别表示位置和姿态。
