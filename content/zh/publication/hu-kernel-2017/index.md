---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Kernel optimization for short-range molecular dynamics
subtitle: ''
summary: ''
authors:
- Changjun Hu
- Xianmeng Wang
- Jianjiang Li
- Xinfu He
- Shigang Li
- Yangde Feng
- Shaofeng Yang
- He Bai
tags: []
categories: []
date: '2017-02-01'
lastmod: 2023-01-04T22:29:03+08:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
publishDate: '2023-01-04T14:29:11.845539Z'
publication_types:
- '2'
abstract: To optimize short-range force computations in Molecular Dynamics (MD) simulations,
  multi-threading and SIMD optimizations are presented in this paper. With respect
  to multi-threading optimization, a Partition-and-Separate-Calculation (PSC) method
  is designed to avoid write conflicts caused by using Newton’s third law. Serial
  bottlenecks are eliminated with no additional memory usage. The method is implemented
  by using the OpenMP model. Furthermore, the PSC method is employed on Intel Xeon
  Phi coprocessors in both native and offload models. We also evaluate the performance
  of the PSC method under different thread affinities on the MIC architecture. In
  the SIMD execution, we explain the performance influence in the PSC method, considering
  the ‘‘if-clause’’ of the cutoff radius check. The experiment results show that our
  PSC method is relatively more efficient compared to some traditional methods. In
  double precision, our 256-bit SIMD implementation is about 3 times faster than the
  scalar version.
publication: '*Computer Physics Communications*'
doi: 10.1016/j.cpc.2016.07.010
links:
- name: URL
  url: https://linkinghub.elsevier.com/retrieve/pii/S0010465516301928
---
