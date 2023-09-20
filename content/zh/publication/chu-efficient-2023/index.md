---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Efficient Algorithm Design of Optimizing SpMV on GPU
subtitle: ''
summary: ''
authors:
- Genshen Chu
- Yuanjie He
- Lingyu Dong
- Zhezhao Ding
- Dandan Chen
- He Bai
- Xuesong Wang
- Changjun Hu
tags: []
categories: []
date: '2023-01-01'
lastmod: 2023-09-20T14:45:21+08:00
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
publishDate: '2023-09-20T06:47:53.258484Z'
publication_types:
- '1'
abstract: 'Sparse matrix-vector multiplication (SpMV) is a fundamental building block
  for various numerical computing applications. However, most existing GPU-SpMV approaches
  may suffer from either long preprocessing overhead, load imbalance, format conversion,
  bad memory access patterns. In this paper, we proposed two new SpMV algorithms:flat
  andline-enhance, as well as their implementations, for GPU systems to overcome the
  above shortcomings. Our algorithms work directly on the CSR sparse matrix format.
  To achieve high performance: 1) for load balance, theflat algorithm uses non-zero
  splitting andline-enhance uses a mix of row and non-zero splitting; 2) memory access
  patterns are designed for both algorithms for data loading, storing and reduction
  steps; and 3) an adaptive approach is proposed to select appropriate algorithm and
  parameters based on matrix characteristics. We evaluate our methods using theSuiteSparse
  Matrix Collection on AMD and NVIDIA GPU platforms. Average performance improvements
  of 424%, 741%, 49%, 46%, 72% are achieved when comparing our adaptive approach with
  CSR-Vector, CSR-Adaptive, HOLA, cuSparse and merge-based SpMV, respectively. In
  bandwidth tests, our approach can also achieve a high memory bandwidth, which is
  very close to the peak memory bandwidth.'
publication: "*Proceedings of the 32nd International Symposium on High-Performance\
  \ Parallel and Distributed Computing (HPDC '23), June 16–23, 2023, Orlando, FL,\
  \ USA*"
doi: 10.1145/3588195.3593002
links:
- name: URL
  url: http://doi.org/10.1145/3588195.3593002
- name: "Conference Site"
  url: https://www.hpdc.org/2022/program/technical-sessions/
- name: "CCF B"
  url: "#"
- name: "News"
  url: "/post/2023-hpdc-spmv-paper/"

url_code: 'https://github.com/hpcde/spmv-acc/'
url_slides: https://drive.google.com/file/d/1U4iajY9dF0QfSTCL1pW7L0TTsqs85KaS/view?usp=share_link
---
