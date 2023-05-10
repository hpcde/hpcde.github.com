---
title: "喜讯：胡长军教授团队论文被高性能计算领域重要会议 HPDC 2023 接收"
date: 2023-05-10T21:01:00+08:00
# authors: GPU team
draft: false
authors:
  - admin
---

日前，课题组胡长军教授团队储根深博士等人完成的论文 “Efficient Algorithm Design of Optimizing SpMV on GPU” 被 HPDC 2023 接收。

[高性能并行和分布式计算国际研讨会](https://hpdc.org)（International Symposium on High-Performance Parallel and Distributed Computing，HPDC）旨在介绍有关高性能计算并行和分布式系统设计、实现、评估和使用的最新研究，是大型计算机研究中久负盛名的会议之一（[CS-Ranking](https://csrankings.org)上列出的高性能计算领域三大顶会之一）。  
HPDC 2023 将于6月中旬在美国弗罗里达州奥兰多市召开，该会议从 100 多篇投稿论文中，最终评审出 22 篇高质量论文录用。

<!--more-->

论文 “Efficient Algorithm Design of Optimizing SpMV on GPU” 面向 GPU 架构上的稀疏向量乘（SpMV）这一重要 kernel，开展了新的算法设计与性能优化，提出了两个新的高效 SpMV 并行算法并通过自适应的方式进行组合，将 SpMV 的性能进行了大量提升，突破了前述算法的性能纪录。

一直以来，稀疏矩阵向量在科学计算中发挥着重要作用，自 GPU 出现以来的数十年里，高性能计算的科研人员和高性能计算工程师们一直在开展 SpMV 的性能调优，以不断逼近硬件性能极限。
本文提出的SpMV 的算法，对 GPU 上的负载均衡、访存性能、高速片上缓存和调度开展了深入研究。

![line-enhance 算法](/images/news/2023-spmv-hpdc23/spmv-line-enhance.svg)
*本论文提出的新算法示意图 (其一的 line-enhance 算法)*

最终实现的算法相对于目前的 SOTA （state of the art） 算法，
性能分别有了424%（对比 CSR-Vector 算法）, 741% （对比 CSR-Adaptive 算法）, 49%（对比 HOLA 算法）, 46%（对比 cuSparse 算法）, 72%（对比 merge-based SpMV 算法）的提升。
该成果得到审稿人的充分肯定，并评价说 “Performance improvement compared to cuSparse and ROCm are impressive.”（注：cuSparse 与 ROCm 分别是 NVIDIA 和 AMD GPU的系统库）。

![](/images/news/2023-spmv-hpdc23/spmv-vs-cub-speedup.svg)
*图：本论文提出的新算法性能与CUDA 生态的 cub 库的性能对比 (纵坐标为加速比，横坐标为稀疏矩阵算例，按矩阵非零元素排列，大于1表述我们算法性能更优)*

团队一直以来面向国产超算开展高性能计算软件、算法库的开发与性能优化工作，目前该系列算法已经适配曙光超算的 DCU 架构，期待后续该系列算法可以在国产超算生态中发挥重要作用。

---
论文信息：
```bib
# For github user: you can also click the link in this repository landing page at the right sidebar, with the label "Cite this repository."
@inproceedings{chu_spmv_gpu:_2023,
 title = {Efficient Algorithm Design of Optimizing SpMV on GPU},
 isbn = {979-8-4007-0155-9/23/06},
 url = {http://doi.org/10.1145/3588195.3593002},
 doi = {10.1145/3588195.3593002},
 language = {en},
 urldate = {2023-6-20},
 booktitle = {Proceedings of the 32nd International Symposium on High-Performance Parallel and Distributed Computing (HPDC '23), June 16--23, 2023, Orlando, FL, USA},
 publisher = {ACM Press},
 author = {Chu, Genshen and He, Yuanjie and Dong, Lingyu and Ding, Zhezhao and Chen, Dandan and Bai, He and Wang, Xuesong and Hu, Changjun},
 year = {2023},
 numpages = {14},
 series = {HPDC '23},
 address = {Orlando, Florida},
 location = {Orlando, FL, USA},
 pages = {1--14},
}
```

论文链接：[http://doi.org/10.1145/3588195.3593002](http://doi.org/10.1145/3588195.3593002)。
