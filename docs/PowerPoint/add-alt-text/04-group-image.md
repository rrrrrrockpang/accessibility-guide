---
title: Group Images on PowerPoint
layout: default
parent: Add Alternative Text
grand_parent: PowerPoint Accessibility
nav_order: 4
---

# Group Images on PowerPoint
{: .fs-9 }

For complex diagrams that have many sub-images, if you don’t group the pictures, the screen reader users will likely (and unnecessarily) be overwhelmed and confused. This page includes two approaches to group images on PowerPoint.

1. [Why do we need to group images?](#why-do-we-need-to-group-images)
2. [Approach 1: Group the images on PowerPoint](#approach-1-group-the-images-on-powerpoint)
3. [Approach 2: Save as Picture](#approach-2-save-as-picture)

## Why do we need to group images?

Let’s walk through the example below about Singular Value Decomposition (SVD). As you can see it’s an SVD equation $A = U \Sigma V^T$, but there are just so many unorganized pointers such as $m$ rows, $n$ columns, approximation sign ($\approx$), $r$ columns/rows, etc. You can also see the messiness on the Selection Pane. (Please look at the reading order section, it is important!). Now, there are two ways to resolve this issue.

<img src="{{site.baseurl}}/assets/images/PowerPoint/alt-text-6.png" alt='This is a screenshot of a powerpoint slide and the Selection Pane. On the left, there is a powerpoint slide titled "Reducing Matrix Dimension", followed by text description, and then followed by math equation A \approx U \Sigma V^T. All three components are laid out in matrix format to make it easy to comprehend. The rows and columns number are denoted in various numbers. on the right is the "Selection Pane" pane. In the pane, 11 textboxes of the components from the left slide are selected. '>

## Approach 1: Group the images on PowerPoint.

### 1. Select each of the pictures you want to group. 

Right-click on the selected images/texts, etc → **View Alt Text …** → **Mark as decorative**. Doing so will make the screen reader skip focusing on the individual images, and just focus on the group. We do this because we don’t want the screen reader to go to the individual components again. We just want to read the grouped component as a whole.

<img src="{{site.baseurl}}/assets/images/PowerPoint/alt-text-7.png" alt='This is a screenshot of a powerpoint slide and the Alt Text Panel. on the left, there is a powerpoint slide titled "Reducing Matrix Dimension", followed by text description, and then followed by math equation A \appro U \Sigma V^T. All three components are laid out in matrix format to make it easy to comprehend. The rows and columns number are denoted in various numbers. On the right is the "Alt Text" pane. In the pane, "Mark as decorative" is selected.'>

### 2. Group the components.

Right-click on the selected images/texts, etc → **Group** → **Group**. Yes, "Group" under "Group".

<img src="{{site.baseurl}}/assets/images/PowerPoint/alt-text-8.png" alt='The same powerpoint slide as above, but all components are selected. Then right button is clicked. In the context menu, "Group" is selected. Then in the sub-menu, "group" is selected again. (Yes, "group" under "Group")'>

### 3. Add alt text to the group.

At this step, all the components should be in a group. You need to add alt text to the group. 

<img src="{{site.baseurl}}/assets/images/PowerPoint/alt-text-9.png" alt='This is a screenshot of a powerpoint slide and the Alt Text Panel. On the left, there is the same powerpoint slide titled "Reducing Matrix Dimension". This time the math equation components (formerly 11) are grouped into one giant component. on the right is the "Alt Text". In the alt text text area it says "An equation of SVD (Singular Value Decomposition). The point is that we can approximate an original matrix by an equation of three smaller matrices. The original matrix A can be approximated by Matrix U multiply \Sigma matrix multiple the transpose of the V matrix." '>


## Approach 2: Save as Picture

### 1. Select the components and save as picture

Select the pictures you want to group → **Save as Picture …** 

<img src="{{site.baseurl}}/assets/images/PowerPoint/alt-text-10.png" alt='The same powerpoint slide as above, but all components are selected. Then right button is clicked. In the context menu, "Save as Picture" is selected. '>

### 2. Drag the saved picture from your folder to this slide. 

If you want the saved picture to go back to where it was, don’t delete the original components yet. You can overlay the saved picture with the original components. When they overlap, **cut** the saved picture → select the original components → delete → paste the saved picture. You are all set now. 

### 3. Add alt text to the picture.

You can just add alt text to the new component as an image!

