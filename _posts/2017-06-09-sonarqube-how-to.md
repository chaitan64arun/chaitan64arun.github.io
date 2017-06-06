---
layout: post
title:  SonarQube Developer's interpretation
tags:
- Technology
- Code Quality
- Code Inspection
---

Recently our company has started using [SonarQube][SonarQube][2086f6ac] an continuous inspector of code quality.
  [2086f6ac]: https://www.sonarqube.org/ "SonarQube"

It's primary aim is to quantify code quality using static analysis and compare it periodically to alert developers.
The UI is very easy to use and self explanatory. It has a dashboard where a developer can check the statistics about his/her project.

But I have observed that many developers neglect to either check these metrics or take action. I have asked several developers and to my surprise the second most popular reason is - developer doesn't know how to use it. So, I decided to make this tutorial about how to interpret SonarQube Results.

The first thing to look at in SonarQube is [Quality Gate][https://docs.sonarqube.org/display/SONARQUBE62/Quality+Gates].
