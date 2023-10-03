---
title: Computational Notebook Accessibility
layout: default
nav_order: 3
has_children: true
permalink: /docs/notebook
---

# Computational Notebook Accessibility
{: .fs-9 }

How to Make Computational Notebooks Accessible (e.g., Google Colab)?
{: .fs-6 .fw-300 }

In CS classes, we often use computational notebooks (e.g., [Google Colab](https://colab.research.google.com/?utm_source=scs-index)) to provide interactive learning experiences to implement and test algorithms. These notebooks are interactive and allow students to run code snippets and see the results immediately. However, these notebooks are not accessible to screen reader users (at least for now).

To make Colab assignments more accessible, you can 

* **Organize your Colab activity with clear division.** This will be helpful for all students to make sense of the notebook and especially helpful to prepare accessible content.

* **Host your Colab notebook as Python scripts.** The students can work on a server (e.g., CSE servers accessible to students like attu1) or locally. We recommend a shared environment that can be tested by the course staff ahead of time since library incompatibilities etc. can present significant barriers to students. Working outside of interactive notebook environments means that students with visual impairment need to re-run entire programs rather than just single snippets/cells. This can take substantially more time, especially when the program is slow (e.g., ML on larger datasets).

In this section, we will show you how to make computational notebooks accessible. 
