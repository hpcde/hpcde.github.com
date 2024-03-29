---
title: "实验室团队在第二届 “先导杯” 计算应用大奖赛中获“SpMV”赛道二等奖"
date: 2021-10-17T08:00:00+08:00
# authors: GPU team
draft: false
authors:
  - admin
---

10月15日，中科曙光和百度公司等联合主办的第二届“先导杯”计算应用大奖赛圆满落幕。由实验室成员（储根深（队长）、何远杰、丁哲昭、董玲玉、邢龙岳、戴潮虎、卢旭）组成的"PHP是最好的编程语言"战队斩获“SpMV”赛道二等奖，
斩获奖金6万元。
<!--more-->

![](http://scce.ustb.edu.cn/attach/file/xinwentongzhi/xueyuanxinwen/2021-10-17/2ccaee86d5dfda1d17c34fcf35921944.jpg)

第二届“先导杯”计算应用大奖赛于2021年4月至10月举办，该赛专注于基础核心算法的探究、应用领域原创性开发的培育，以及软件环境、学科应用等方面瓶颈的突破。
多所重点高校、科研机构、知名企业的1500多名选手、1000余支战队积极参与，共产出数百份创新应用的移植、优化成果，涉及二十几个领域的交叉应用，为我国计算软件应用的生态建设添砖加瓦。
大赛共分为七个赛道，每个赛道设置一等奖一个，二等奖两个，三等奖三个。
其中SpMV（稀疏矩阵向量乘）赛道要求采用异构编程加速SpMV，重点关注双精度实数在异构计算平台上的计算性能。
实验室"PHP是最好的编程语言"战队突破重重难关，提出了适用于不同矩阵特征的创新性算法，在曙光计算平台上完成了SpMV的高效实现，创建了通用的 [SpMV-acc](https://github.com/hpcde/spmv-acc) 算法库，算法库中集成了适用于不同矩阵特征的多计算种策略，测试结果相对 rocSparse 算法库性能提升16%-70%，获得了较高的浮点计算性能和访存带宽。
代码现已在github开源：https://github.com/hpcde/spmv-acc (Apache-2.0 协议)。

<p style="text-align:center">
  <img src="/images/news/pra-2021/spmv-performance.webp"/>
</p>

![](http://scce.ustb.edu.cn/attach/file/xinwentongzhi/xueyuanxinwen/2021-10-17/fb4742f5cf2288a07646ffc928780fd9.jpg)
