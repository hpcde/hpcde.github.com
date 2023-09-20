---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'Testing high performance numerical simulation programs: experience, lessons
  learned, and open issues'
subtitle: ''
summary: ''
authors:
- Xiao He
- Xingwei Wang
- Jia Shi
- Yi Liu
tags: []
categories: []
date: '2020-07-01'
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
publishDate: '2023-01-04T14:29:12.338426Z'
publication_types:
- '1'
abstract: High performance numerical simulation programs are widely used to simulate
  actual physical processes on high performance computers for the analysis of various
  physical and engineering problems. They are usually regarded as non-testable due
  to their high complexity. This paper reports our real experience and lessons learned
  from testing five simulation programs that will be used to design and analyze nuclear
  power plants. We applied five testing approaches and found 33 bugs. We found that
  property-based testing and metamorphic testing are two effective methods. Nevertheless,
  we suffered from the lack of domain knowledge, the high test costs, the shortage
  of test cases, severe oracle issues, and inadequate automation support. Consequently,
  the five programs are not exhaustively tested from the perspective of software testing,
  and many existing software testing techniques and tools are not fully applicable
  due to scalability and portability issues. We need more collaboration and communication
  with other communities to promote the research and application of software testing
  techniques.
publication: '*Proceedings of the 29th ACM SIGSOFT International Symposium on Software
  Testing and Analysis*'
doi: 10.1145/3395363.3397382
links:
- name: URL
  url: https://dl.acm.org/doi/10.1145/3395363.3397382
- name: "CCF A"
  url: ""
---
