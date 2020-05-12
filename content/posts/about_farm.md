---
title: "About the Farm Cluster"
date: 2019-06-25T15:20:30-07:00
description: "The UC Davis CA&ES Farm Cluster"
#thumbnail: "img/placeholder.jpg" # Optional, thumbnail

lead: "CSE Team" 
# Lead is the author, use "Helpdesk", "Admins", or "yourfirstname"

disable_comments: true # Optional, disable Disqus comments if true
authorbox: false # Optional, enable authorbox for specific post
toc: false # Optional, enable Table of Contents for specific post
mathjax: false # Optional, enable MathJax for specific post
categories:
  - "information"
  - "System"
tags:
  - "info"
  - "system"

draft: false
---
Farm is a Linux-based supercomputing cluster for the College of Agricultural and Environmental Sciences at UC Davis. Designed for
both research and teaching, it is a significant campus resource primarily for CPU and RAM-based computing, with a wide selection
of centrally-managed software available for research in genetics, proteomics, and related bioinformatics pipelines, weather 
and environmental modeling, fluid and particle simulations, geographic information system(GIS) software, and more. 

<!--more-->

Farm Hardware
------------
Farm is an evolving cluster that changes and grows to meet the current needs of researchers, and has undergone three phases, 
with Farm III as the most recent evolution. 

Farm III consists of 32 parallel nodes with 64 CPUs and 256GB RAM each, plus 17 "bigmem" nodes with 96 CPUs and
1TB RAM each. All Farm III bigmem and newer parallel nodes and storage are on EDR/100Gbit interconnects. Older parallel nodes and storage are on FDR/55Gbit.

Farm II consists of 95 parallel nodes with 24 CPUs and 64GB RAM each, plus 9 "bigmem" nodes with 64 CPUs and 512GB RAM each,
and 1 additional node with 96 CPUs and 1TB RAM. Farm II nodes are on QDR/32Gbit interconnects.

Hardware from both Farm II and Farm III are still in service; Farm I has been decommissioned as of 2014.

Farm also has multiple fileservers with over 5.3PB of storage space total.

Access to Farm 
--------------
All researchers in CA&ES are entitled to free access to 8 nodes with 24 CPUs and 64GB RAM each (up to a maximum
of 192 CPUs and 512GB RAM) in the low, medium, and high priority batch queues, as well as 1TB storage space. 

Additional usage may be purchased by contributing to Farm III by buying nodes and/or storage space at set rates.

Contributors always receive priority access to the resources that they have purchased within one minute with the
"one-minute guarantee." Users can also request additional unused resources on a "fair share" basis--someone 
who contributes twice as much will be able to use twice as many unused resources in the medium or low partitions.

Farm Administration
-------------------
Farm hardware and software are administrated by the [CSE Team](http://ceylon.cse.ucdavis.edu/posts/about/).


Current Rates
-------------
As of 2019, the rates for Farm III:

* Parallel node: 48 cores/96 threads, 256GB RAM (low2, med2, high2 partitions) - $8,800
* Bigmem node: 48 cores/96 threads, 1TB RAM (bml, bmm, bmh partitions) - $22,7000
* GPU node: dual-socket Xeon 4114, Nvidia Tesla V100 - $17,500
* Partial (1/8th) GPU node: 1 of 8 Titan RTX 24GB, 3 of 24 Xeon Cores, 96GB of 768GB RAM - $4,000
* Storage: 10TB for 5 years (does not include backups) - $1,000
* Equipment purchases not using above rates - $275/year per rack unit


For more information about buying into Farm, contact [Adam Getchell](mailto:acgetchell@ucdavis.edu) or the [Helpdesk](mailto:help@cse.ucdavis.edu).


