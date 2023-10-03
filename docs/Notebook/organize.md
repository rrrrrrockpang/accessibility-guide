---
title: Organize Your Computational Notebook
layout: default
nav_order: 1
parent: Computational Notebook Accessibility
permalink: /docs/notebook/organize
---

# How to Organize Your Computational Notebook?
{: .fs-9 }

In this section, we will provide an example to illustrate how to organize your computational notebook. This will be helpful for all students to make sense of the notebook and especially helpful to prepare accessible content.

### 1. Check the table of contents.
Check the table of contents on your Colab left bar. Make sure each section has a clear title and description. 

<img src="{{site.baseurl}}/assets/images/Notebook/colab-1.png" alt='This is a screenshot of the Google Colab interface. On the left, it has a table of contents of the document (The table has two sections. The first section is "CSE 547 - Colab 0", which has a subsection "Setup". The second section is "Vietnam War" which includes 4 subsections of questions); On the right, it has notebook including Python code snippets and texts.'>


### 2. Divide the Colab Document into Separate Python Scripts.

A good guide to organize your Colab notebook is to divide it into separate Python scripts. Migrate the sections into separate Python scripts. The goal here is that screen reader users can work on the modular script for each section. 

<img src="{{site.baseurl}}/assets/images/Notebook/colab-2.png" alt='This is a screenshot of a directory on github. It includes a folder (data), one markdown file (question.md), and 5 python files (intro.py, section_1.py, section_2.py, section_3.py, section_4.py).' width="400px">

{: .note }
You might realize that we created a separate `data` folder in the github directory compared to `drive = GoogleDrive(gauth)` which is unique to Google Colab. Make sure that you share your data file (e.g., Google Drive) so that everyone can have access to it.

### 3. Run the notebook to make sure everything works.

Always to run the notebook before releasing the homework. Also, host your notebook on a shared environment that can be tested by the course staff ahead of time since library incompatibilities etc. can present significant barriers to students.
