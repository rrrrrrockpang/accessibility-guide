---
title: Add Latex for Math Notations
layout: default
parent: PowerPoint Accessibility
nav_order: 4
---

# Add Latex for Math Notations
{: .fs-9 }

Make sure to add latex for complex math notation if you just include a screenshot/picture of the math. Some students with visual impairments are able to read latex representations. Consider the example about TF-IDF below: 

<img src="{{site.baseurl}}/assets/images/PowerPoint/latex-math-1.png" alt='This is a screenshot of a powerpoint slide and the Alt Text Panel. On the left, there is a powerpoint slide with a few formulas about "Jaccard Similarity Metric", "Cosine Similarity Metric", and "Pearson Correlation Coefficient". Next to each formula are some explanation that would be animated to display. On the right, the selection pane displays the reading orders of these elements on the powerpoint slide' width="400px">

In the example, there are texts, inline math symbols (e.g., $f_{ij}$), math equation as one line (e.g., $TF_{ij} = \frac{f_{ij}}{max_{k}f_{kj}}$), arrows, and explanation. It involves many components and adding alt text to each single component can be challenging both for the authors and the readers. 

To resolve this problem, you should:

* Keep your original slide (yes, regardless of how many components).
* Mark all components decorative.

<img src="{{site.baseurl}}/assets/images/PowerPoint/latex-math-3.png" alt='This is the same screenshot of the powerpoint and the alt text panel as above. This time, all the math components and the associated texts are marked decorative on the alt text panel.' width=400>

* Create another white box and add alt text as LaTeX to it.

<img src="{{site.baseurl}}/assets/images/PowerPoint/latex-math-2.png" alt='This is the same screenshot of the powerpoint and the alt text panel as above. This time, a white box is highlighted and the alt text for this empty box is the math and text that we marked decorative previously.' width=400>

{: .note }
[LaTeXiT](https://www.chachatelier.fr/latexit/) is a great tool to quickly iterate on the LaTeX formula as you work on your slides.
