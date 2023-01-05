---
title: "实验室大规模并行分子动力学模拟软件 MISA-MD 获\"天河之星\"优秀应用奖"
date: 2020-12-04T06:50:32+08:00
# authors: MISA-MD team
draft: false
authors:
  - admin
---

<a class="github-button" href="https://github.com/misa-md" data-size="large" aria-label="Follow @misa-md on GitHub">Follow @misa-md team</a>

近日，实验室开发的大规模并行分子动力学模拟软件 MISA-MD 获得国家超算广州中心的"天河之星"优秀应用奖，
团队成员前往广州参加用户大会，并出席优秀应用颁奖典礼。
<!--more-->
据悉，本次"天河之星"优秀应用奖，面向全国多个应用领域征集，并从中遴选出 20 个优秀应用。

此次获奖的分子动力学软件 MISA-MD 是团队主持开发的 MISA 系列材料多尺度模拟软件中的一款，
其可以利用复杂的 EAM 势函数来模拟级联碰撞导致的初始缺陷产生过程。
实验室团队成员联合中国原子能科学院研究团队，在天河2号超算上利用 MISA-MD 程序，完成了不同 PKA 能量、方向下的级联碰撞应用算例。
通过模拟与结果分析，MISA-MD 获得了不同 PKA 能量下的铁基材料受到高能中子轰击后的缺陷演化过程。并获得级联碰撞过程之后的稳定缺陷空间分布，为后续更长时间的缺陷演化模拟方法提供了初始输入与必要参数。通过应用大规模高性能的 MD 模拟，有望进一步突破时空尺度限制，进行更大时空尺度的材料演化模拟，揭示材料微观演化机理。

|  |  |
| -- | -- |
| <p style="text-align:center"><img src="/images/news/tianhe-star/exhibition.jpg" width="300px" /></p> |  <p style="text-align:center"> <img src="/images/news/tianhe-star/star.jpg" width="250px" /></p> |

团队自研的 MISA-MD 程序采用自己设计的粒子存储数据结构和邻居粒子的查找遍历算法，大幅提高 MD 性能与规模。相对于经典的分子动力学模拟软件lammps，MISA-MD在天河2号超算上，内存节省约超过 **60%**，计算性能提升约 **10%～20%**。
面向材料级联碰撞过程的模拟，团队专门开发了级联碰撞模拟模块，相对于其他分子分子动力学软件，进行级联碰撞模拟更容易操作且用户友好。
此外，MISA-MD 还提供了多平台计算支持，目前 MISA-MD 支持多款国产超算系统，包括纯CPU架构、GPU/DCU加速卡、神威从核。

目前, MISA-MD 源代码已经在 github 平台上开源，采用BSD 开源协议：[https://github.com/misa-md/misa-md](https://github.com/misa-md/misa-md) 。

<p style="text-align:center">
  <img src="/images/news/tianhe-star/team.jpg" width="320px" />
</p>
