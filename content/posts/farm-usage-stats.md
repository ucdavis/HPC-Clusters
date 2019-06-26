---
title: "Farm Usage Stats"
date: 2019-05-22T15:35:11-07:00
description: "Interesting statistics for the Farm cluster"
#thumbnail: "img/placeholder.jpg" # Optional, thumbnail

lead: "Tim" 
# Lead is the author, use "Helpdesk", "Admins", or "yourfirstname"

disable_comments: true # Optional, disable Disqus comments if true
authorbox: false # Optional, enable authorbox for specific post
toc: false # Optional, enable Table of Contents for specific post
mathjax: false # Optional, enable MathJax for specific post
categories:
  - "blog"
tags:
  - "blog"

draft: false
---
I recently ran some usage statistics on Farm, our biggest cluster, to get an idea of how
it is being used. 

<!--more-->

(Before continuing, please note that these are experimental and estimated results, and as such 
may be subject to refinement, changes, or deletion at any given point.)

First, let's take a look at the usage by the top 50 users.

|Date Range    |CPU-Years   |CPU-Days      | CPU-Hours        |    CPU-Minutes    |
|----------------|------------|--------------|------------------|-------------------|
|**01/01-05/19** |**610.09**  |**222,681.3** |**5,344,347.05**  |**320,660,823**    |
|01/01-04/01     | 417.93     | 152,542.82   | 3,661,027.7      | 219,661,662.0     |
|05/01-05/16     | 68.34      |   4,944.72   | 598,673.3        | 35,920,398        |

A CPU-year is one CPU at 100% duty for one year.

Metrics from here on out get a little tricky. I'll be making a few assumptions and back-of-the-envelope shortcuts that won't
result in exact numbers, but should land us in a solid ballpark range.

We'll say that Farm has about 6,000 CPUs after adding about 1,500 in April/May. That's 6,000 CPU-years of
total processing theoretically available across the entire cluster anually. That's also assuming 100% availability of 100% of
assets. Which is, of course not always the case--given the fickleness of hardware and software, the vagaries of funding
and the purchasing process, maintenance windows, and so on. However, let's back things up a little bit. 

We'll go to the beginning of April for to remove that sudden boost of 1,500 CPUs. That's a theoretical maximum of 
4,500 CPU-Yrs for the year. 

Based on that, the period from January 1-April 1 has a theoretical maximum of 1,120.5
CPU-Yrs available. 

Let's look at total usage stats for all users:

Slurm sreport cluster utilization start=01/01/19 end=04/01/19:

| Type        | CPU-Years   | CPU-Days     | CPU-Hours      | CPU-Minutes        |
|-------------|-------------|--------------|----------------|--------------------|
| Reported    | 1,179.18    | 430,400.57   | 10,329,613.5   | 619,776,819.0      |
| Allocated   | 435.93      | 159,115.41   | 3,818,769.9    | 229,126,194.0      |


Slurm's sreport command is a little vague about what "reported" means, but the definition I'm going with
is that it's the approximate total CPU-Years available for use in a time period, and "allocated"
is what was actually used by jobs during that time period.

(Our reported CPU-Yrs total is a little higher than our calculated theoretical maximum CPU-Yrs, but remember, that was just
an estimate. The difference works out to about one Farm III node or two older Farm II nodes.)

The tables reveal that the top 50 users of farm are responsible for the majority of cycles: about 418 CPU-Yrs
out of 436, or 96% of cluster use.

The biggest single user was responsible for about 75 CPU-Yrs alone (17% of cluster use). The top 3 users together accounted 
for 186 CPU-Yrs, or about 43% of cluster use. 

Conclusions
--------------
There are a couple takeaways that I read from all this. First, we can be pretty proud of our uptime for Farm. 
We're very close to our theoretical maximum cycles available, meaning we're keeping nodes up and ready to use
as much as possible, all while using minimal staff and low overhead. And while Farm is our largest cluster, 
it's not our only cluster -- we're currently managing nine other clusters, as well. 

It also looks like Farm is running at somewhere around 1/3rd to 1/2 capacity on average, which isn't bad at all. 
Usage often happens in bursts, so while there are times when almost all of the CPU cycles are booked, for the most part 
we almost always have some extra cycles available whenever someone needs them--even without our "one-minute guarantee."
That's a good sign that the cluster is healthy, seeing regular use, and is at the right size to meet the needs of the current users.


-TDT@CSE

