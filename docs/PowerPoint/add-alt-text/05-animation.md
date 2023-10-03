---
title: Make Animation Accessible
layout: default
parent: Add Alternative Text
grand_parent: PowerPoint Accessibility
nav_order: 5
---

# Make Animation Accessible
{: .fs-9 }

It is common to have animation on your slides, but screenreader users rely on the correct **reading order** and **detailed alt text**. 

In the example below, the slide sequentially displays the formulas for 'Jaccard Similarity Metric', 'Cosine Similarity Metric', and 'Pearson Correlation Coefficient'. With each animation, the corresponding examples (i.e., $r_x$, $r_y$)  are revealed in green text on the right-hand side of the slide.

<img src="{{site.baseurl}}/assets/images/PowerPoint/alt-text-12.png" alt='This is a screenshot of a powerpoint slide and the selection pane. On the left, there is a powerpoint slide with a few formulas about "Jaccard Similarity Metric", "Cosine Similarity Metric", and "Pearson Correlation Coefficient". Next to each formula are some explanation that would be animated to display. On the right, the selection pane displays the reading orders of these elements on the powerpoint slide'>

### 1. Check the reading order.

Make sure that the reading order follows the animation order: the first element in the reading order should be the first element animated. Below shows the animation order in the `Animation Pane`.

<img src="{{site.baseurl}}/assets/images/PowerPoint/alt-text-11.png" alt='This is a screenshot of the animation pane. On top it displays a green triangle followed by text "Play All". It is followed by an up and a down arrow and a delete button. Below this row shows "animations". Each animation is one row (it has 5 rows on the screenshot). Each animation has the animation order (0, 1, 2, ...) followed by the title of these animation. (Each animation can consist of multiple text chunks on a powerpoint). ' width=300>

### 2. Avoid adding animation inside of one single text box.

Don’t add animation inside of one single text box. For example, don’t lump all three similarity metrics into one giant text box and add animation inside. Instead, create three text boxes, each of which represents one metric. This makes it easier to adjust the reading order. 