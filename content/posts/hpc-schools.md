---
title: "HPC Department Comparisons"
date: 2019-05-01T12:26:25-07:00
draft: false
description: "Comparing HPC Departments Across Schools"
#thumbnail: "img/placeholder.jpg" # Optional, thumbnail
lead: "Tim"
disable_comments: true # Optional, disable Disqus comments if true
authorbox: true # Optional, enable authorbox for specific post
toc: false # Optional, enable Table of Contents for specific post
mathjax: false # Optional, enable MathJax for specific post
categories:
  - "information"
  - "blog"
tags:
  - "info"
  - "blog"
---
We were curious about what other HPC departments looked like at universities across the USA in terms of staffing versus
the amount of hardware managed, so I gathered some information from publicly-available university websites. Here's a chart comparing
them. 

<!--more-->


|   Department                                                                 | Staff |Clusters| Nodes   | CPUs |  GPUs   |
|------------------------------------------------------------------------------|----------|--------|---------|----------|--------|
| [Yale University](http://research.computing.yale.edu/)                       | **19**   | **5**  |**3005**  |**28504**|**78**         |
|                                                                              |          |        | 1755    | 11620    | 40            |
|                                                                              |          |        |  267    | 5368     | 38            |
|                                                                              |          |        |  754    | 6384     | 0             |
|                                                                              |          |        |  169    | 3548     | 0             |
|                                                                              |          |        |  60     | 1584     | 0             |
| [UMN - Minnesota Supercomputing Institute](https://www.msi.umn.edu/)               | **10**   | **2**  |**2539** |**27496** | **80**  |
|                                                                              |          |        | 1142    | 9712     | 0             |
|                                                                              |          |        | 741     | 17784    | 80            |
| [UC Irvine - RCIC](https://hpc.oit.uci.edu/)                                 | **7**    | **1**  |**280**  |**12000** |**48**         |
| [OSU - Ohio Supercomputing Center](https://www.osc.edu/services/cluster_computing) | **38**   | **3**  |**1100** |**38482** | **244** |
|                                                                              |          |        | 824     | 23392    | 160           |
|                                                                              |          |        | 252     | 10240    | 64            |
|                                                                              |          |        | 41      | 4800     | 20            |
| [College of Charleston](http://compsci.cofc.edu/about/hpc.php)               |**2+?**   |**2**   |**42**   |**340**   |**0**          |
|                                                                              |          |        |  26     | 84       | 0             |
|                                                                              |          |        |  16     | 256      | 0             |
| [University of Connecticut - HPC](http://hpc.uconn.edu)                      | **6**    | **1**  |**360**  |**9000**  |**?**          |
|[University of Connecticut - Bioinformatics](https://bioinformatics.uconn.edu)|**5**     |**1**   |**?**    |**2188**  |**7000 cores** |
| [Washington University in St. Louis](https://research.wustl.edu/core-facilities/center-high-performance-computing) |**2**     |**1**   |**48**   |**2500**  |**64**         |
| [American University](https://www.american.edu/cas/hpc/software.cfm)         |**4**     |**1**   |**17**   |**408**   |**1**          |
| [University of Denver](https://www.du.edu/it/services/research-services/research-computing)                        |**?**     |**1**   |**44**   |**440**   |**2**          |
| [University of Southern California](https://hpcc.usc.edu/)                   |**6+**    |**2**   |**2700** |**14096** |**760**        |
| [Columbia University](https://systemsbiology.columbia.edu/high-performance-computing)                              |**6**     |**1**   |**?**    |**6336**  |**73728 cores**|
| [Georgetown University](https://uis.georgetown.edu/research/high-performance-computing)                            |**?**     |**1**   |**45**   |**800**   |**0**          | 
| [Bioinformatics Core @ UC Davis](https://bioinformatics.ucdavis.edu/)**      |**9**     |**1**?   |**102**?  |**9800**|**65100 cores**|
| [HPC @ UC Davis](http://www.hpc.ucdavis.edu)                                 |**3**     |**10+**  |**520**  |**18176** |**165**        |



**Note:**
 
* This table is intended only as a broad overview of the HPC landscape at various universities. I tried to be as accurate as I could based on what was available online at the sources linked, but my data is only as correct and up-to-date as the websites linked. 

**Definitions:**

* A **node** is the whole computing machine, including one or more processors, RAM, etc. The node count includes general compute nodes, high-memory nodes, and GPU nodes.
* A **CPU** in this chart means a single processor *core* for general computing. A compute node may have one or more multi-core processors.
* A **GPU** is an entire GPU card - unless the only total I could find is the number of GPU *cores* (CUDA cores) that the cluster claims. The core count of a single GPU card 
can range from hundreds in lower-end cards, up to around 5,700 in a higher-end model, with the average being somewhere in the 2,000 to 3,000 range.
 
