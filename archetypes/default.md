---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
description: "Short description of page"
#thumbnail: "img/placeholder.jpg" # Optional, thumbnail

lead: "Helpdesk" 
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

draft: true
---
Page intro/summary goes here
<!--more-->
Page content goes here


