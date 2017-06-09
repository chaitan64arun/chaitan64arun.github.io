---
layout: post
title:  SonarQube Developer's interpretation
tags:
- Technology
- Code Quality
- Code Inspection
---

Recently our company has started using [SonarQube](https://www.sonarqube.org/), a continuous inspector of code quality.

It's primary aim is to quantify code quality using static analysis and compare it with a previous release periodically. The UI is very easy to use and self explanatory. It has a dashboard where a developer can check the statistics about his/her project.

But I have observed that many developers neglect to either *check* these metrics or *take action*. I have asked several developers for the reason. To my surprise the second most popular reason is - developer doesn't know how to use SonarQube. So, I decided to make this tutorial on how should developer interpret SonarQube results.

I will be using [SonarCloud](https://sonarcloud.io/) as an example in this tutorial.

## Projects
The first thing you need to look at in SonarQube is [Projects](https://sonarcloud.io/projects). This can be treated as the summary view for a developer. It is accessible on the header band from any page.

----
 ![dashboard]({{ site.url }}/post-assets/projects.png){:height="303px" width="740px"}
<center><b>This is how it looks like.</b></center>
----
There are four sections that are identified in the above picture. They are filters set up for every metric based on the Grade.

1. Quality Gate
2. Metric (Topic)
3. Grade
4. Project

#### Quality Gates
All metrics in SonarQube are controlled by [Quality Gates](https://docs.sonarqube.org/display/SONARQUBE62/Quality+Gates).
This is generally prepared by your CI team. As a developer we just need to concentrate on **Failed** and **Warning**

#### Metric and Grades
There can be several metrics that are configured by your CI administrator. As a developer we must choose not acceptable grade from each metric and solve each issue

#### Project
This area shows the filtered out projects from our choice of Grade in Quality Gate and Metrics. This area is nicely colour coded and is quite intuitive for a developer to understand.

## Project Dashboard

This page can be accessible from clicking on Project name shown as (4) rectangle in the above picture.
