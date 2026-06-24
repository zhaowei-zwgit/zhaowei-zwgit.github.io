---
title: DP-VGPSU / DP-NAwRL 差异隐私算法框架
date: 2025-06-01
share: false
profile: false
---

独立开发了一套基于 Python/PyTorch 的差异隐私深度学习训练工具包。

<!--more-->

**核心贡献：**

* 实现了"垂直梯度扰动与选择性更新（DP-VGPSU）"算法，利用几何正交分解有效减少了噪声对模型收敛的影响。
* 引入 Q-learning 机制设计了 DP-NAwRL 框架，使系统能够根据训练状态自适应调节噪声注入能量。

**技术栈：** Python, PyTorch, NumPy, Linux, GitHub
