---
layout: default
title: Home
nav_order: 1
description: "This Accessibility Guide for Classes allows you to create class accessible materials for students."
permalink: /
---

# Accessibility Guide for Classes at UW CSE
{: .fs-9 }


This Accessibility Guide for Classes allows you to create class accessible materials for students. 
{: .fs-6 .fw-300 }

by Rock Yuren Pang, Kelly Mack, Venkatesh Potluri, Jennifer Mankoff, Tim Althoff

Table of Contents
{: .no_toc .text-delta }
* [How to use this document](#how-to-use-this-document)
* [Common Barriers in CS Classrooms](#common-barriers-in-cs-classrooms)
* [High-level Takeaway](#high-level-takeaway)


This document gives an overview for instructors and TAs to improve course accessibility for students who are blind or visually impaired (BVI). Whether you don’t know where to start, or want to double-check whether any accessibility concerns may have been missed around your materials, we hope that this document will help you. 
We believe that increasing accessibility makes the course more approachable to all students, though it requires time and effort. This guide will help you make materials accessible more efficiently.

**Intended Audience** Instructors and TAs who are teaching math or CS classes, or anyone who is interested in making accessible course materials including PowerPoint slides, Computational Notebooks, and Homework Write-ups.

This guide was made possible during CSE 547 Fall 2022 at UW, where we collaborated with the Disability Resources for Students (DRS). We hope that this guide will be useful to other instructors and TAs who are interested in making their classes more accessible. We warmly welcome feedback and suggestions to improve this guide.

## How to use this document
{: .fs-6 .fw-300 }

To understand common accessibility barriers in class, you should read the [Common Accessibility Barriers in Classrooms]({{site.baseurl}}/docs/introduction/common_barriers), which outlines issues such as PowerPoint Slides, computational notebooks, homework assignments. Then, we recommend reviewing the specific sections while you are working on the corresponding election of your class.

We also encourage you to show the students examples of your course materials, and specify the tools that may be used for homeworks before they take the class, to identify any remaining barriers early. 

This document focuses on students with visual impairments. here are many  students with a range of disabilities, with a variety of access needs who may require accommodations to succeed in higher education courses. We highly recommend contacting Disability Resources for Students (DRS) at the earliest possible based on your students’ access needs. Note that many campuses’ disability offices are extremely overworked, therefore, we also suggest you give this document a read before reaching out for further questions.

In creating this document, we consulted with Disability Resources for Students and received valuable feedback from Esteban Safranchik, Ken Gu, and Katharina Reinecke. If you have comments, please reach out to Rock Yuren Pang and Tim Althoff (ypang2@cs.washington.edu and althoff@cs.washington.edu). We also welcome additional feedback to improve this document.

## Common Barriers in CS Classrooms
{: .fs-6 .fw-300 }

### PowerPoint Slides
Imagine a blind student trying to understand matrix multiplication in a highly animated PowerPoint slide. The image of a  matrix that you animated happened to be a screenshot from a textbook. Under that scenario, sighted students can easily understand the transformation with the engaging slide, but blind students will likely be completely lost. 

A key takeaway to making PowerPoint slides is not to completely rely on visual cues. You should always consider adding alt text to images, animations, and math notations. If visual cues are important, you can consider augmenting the experience with tactile graphics (braille).

### Computational notebook software, such as Google Colab 
make it easier to collaborate and share code. However, screen reader users cannot access and work with these notebooks, as of this writing. 

To make computational notebooks more accessible, you can easily create separate Python files for each section of your notebook. Additionally, blind users may not be able to create visualizations as homework deliverables. Instead, you can consider having them present the information in an alternate format to test the correctness (e.g., a data table).
 
### Document assignments 
PDFs are often inaccessible to people using screen readers by default. We recommend releasing the Markdown and LaTeX files whenever possible. It is easy to use pandoc convert a Markdown/LaTeX file with math notations to an accessible HTML file supported by MathJax, which works with screen readers (see section 4). 

### In-class activities 
In-class discussions are often accessible by default if they don’t heavily rely on a visual component. However, if your in-class activity needs to focus on a visual element (e.g., discussing the drawbacks between k-means and hierarchical clustering), it helps if you can provide tactile graphics. The Disability Resources for Students can help create these from images and slides.

### Group project
It helps to talk with the students ahead of time to understand what accommodations they might need for a project. In team-based projects, sometimes students like to focus on a certain part of the project, e.g., literature review, giving presentations, or writing, instead of more inaccessible elements (e.g., analyzing visualizations). 

Now that you have a high-level understanding of where you may encounter accessibility issues in your  class, the next few sections are going to expand on each point and guide you through concrete steps to make them more accessible.

## High-level Takeaway
{: .fs-6 .fw-300 }

Here are high-level recommendations on how to proceed in a class to improve accessibility for BLV students.

### Communicate before the quarter. 

To accommodate the needs for different students, we recommend communicating with the students before the quarter. Ask them if they need additional accommodations like accessible PowerPoint and coding/homework setup. 

### Communicate with DRS. 

You should communicate with the DRS if this document doesn’t cover specific needs from students. Also it’s helpful to print out necessary braille materials in the beginning of the quarter. The DRS is helpful and the turnaround is usually within 2 weeks. 

### Make the accessible slides publicly 

Make the accessible slides publicly available on the course website so that all students have the chance to preview the slides if they would like to. Share the accessible materials (e.g., braille) with the students 1 week before the class session.

### Test the server before launching homework or colab activities. 

Before releasing the homework or colab on a server, please test that the code can run on the server without configuration issues. Configuration issues can be significant overhead burdens to BVI students. Any unexpected configuration errors can significantly hurt student’s confidence to succeed in the class. 

### Always adjust needs for individual students. 

Note that each student might have different access needs, and preferences to navigate accessibility barriers. Please discuss with them throughout the course for feedback.
