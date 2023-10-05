---
title: Check Reading Order
layout: default
parent: PowerPoint Accessibility
nav_order: 2
---

# Check Reading Order (Selection Order)
{: .fs-9 }

Reading order is also called selection order in some PowerPoint versions. The Reading Order impacts how a screen reader user reads your slide when they are reviewing it. Correct selection/reading order  ensures that the screen reader will follow your presentation order. (Imagine that’s the order that you’re going to present your slides) If inaccurate, the reading order will confuse the screen readers. For example, for complex slides with multiple text boxes, make sure the conclusion doesn’t show up first or the caption doesn’t follow the wrong graphic. 

When we [checked accessibility in the last section]({{site.baseurl}}/docs/PowerPoint/check-accessibility/#2-check-the-accessibility-panel), we could see that there are 25 errors in the reading order. Now it's time to learn how to **fix the reading order**.

### 1. Launch the selection/reading order panel.
Next to the **Review → Check Accessibility** button, you can find the Selection Pane button.

![Under the same accessibility button in the review tab, one of the drop down list items "selection pane" is highlighted]({{site.baseurl}}/assets/images/PowerPoint/reading-order-1.png)

An alternative way to open this: **Home → Arrange → Selection Pane**

<img src="{{site.baseurl}}/assets/images/PowerPoint/reading-order-2.png" alt='A screenshot of the "selection pane" option highlighted in the "arrange" dropdown' width="400">

### 2. Preview the reading order on the selection pane.

We can find the Selection Pane on the right. It will include all the content that will be parsed by a screen reader. You can see the reading order of the slide on the Selection Pane. 

{: .note } 
The order goes from bottom to top on Mac; it goes from top to bottom on PC. 

Below shows an example of a slide and the reading order on the Selection Pane. The reading order is from bottom to top on Mac.

<img src="{{site.baseurl}}/assets/images/PowerPoint/reading-order-3.png" alt='A screenshot of a powerpoint slide and the selection pane. On the left, there is a powerpoint slide with several text boxes and one image. on the right we see a pane listing out textboxes and images in an ordered list. Right now the title element is at the top of the list and the last textbox (called textbox 6) is at the bottom.'>

### 3. Drag and reorder the components.

To address the inaccurate order, **drag the components to reorder**. For example, the order in the slide above is actually inaccurate. We want to show Title 1 first and then Textbox 6. (i.e., show the title first and then the subtitles and the author.)

You should also **delete unnecessary components**. For example, when we click “Textbox 6”, we actually see an empty box highlighted. It turns out it’s a text box that we forgot to remove when preparing the slide. A redundant textbox like this will likely confuse screen reader users.


### 4. Review the reading order.

When you finish addressing the reading order for all slides, make sure to go back to **Review → Check Accessibility** to see if any warnings are reported. If so, double-check whether you missed a few slides or if you intended your slides to be in a certain order. If the latter you can safely ignore the warnings.
