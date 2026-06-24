---
title: 研究方向
date: 2022-10-24

type: landing

sections:
  - block: slider
    content:
      slides:
      - title: 差异隐私与深度学习隐私保护
        content: 专注于机器学习训练过程中的隐私保护算法设计，特别是通过几何正交分解（Geometric Orthogonal Decomposition）等扰动策略降低噪声能量，优化数据隐私与模型效用（Utility）之间的权衡。
        align: center
        background:
          image:
            filename: ysbh.png
            filters:
              brightness: 0.7
          position: right
          color: '#666'
      - title: 强化学习自适应扰动机制
        content: '探索利用基于价值（Value-based）的强化学习方法（如 Q-learning）构建自适应梯度噪声注入框架，使系统能够根据训练状态自适应调节噪声注入能量，实现隐私保护与模型性能的动态平衡。'
        align: left
        background:
          image:
            filename: mxyh.png
            filters:
              brightness: 0.7
          position: center
          color: '#555'
      - title: 计算机视觉与图像处理
        content: '研究 YOLO 系列目标检测算法及 Real-ESRGAN 超分辨率重建技术在隐私保护场景下的结合与自动化应用，解决隐私扰动后图像特征退化的问题。'
        align: left
        background:
          image:
            filename: fbs.png
            filters:
              brightness: 0.7
          position: center
          color: '#555'
    design:
      # Slide height is automatic unless you force a specific height (e.g. '400px')
      slide_height: ''
      is_fullscreen: true
      # Automatically transition through slides?
      loop: false
      # Duration of transition between slides (in ms)
      interval: 2000
---
