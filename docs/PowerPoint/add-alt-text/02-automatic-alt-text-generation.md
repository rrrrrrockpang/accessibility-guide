---
title: Automatic Alt Text Generation
layout: default
parent: Add Alternative Text
grand_parent: PowerPoint Accessibility
nav_order: 2
---

# Automatic Alt Text Generation
{: .fs-9 }

In the [last section]({{site.baseurl}}/docs/PowerPoint/add-alt-text/how-to-add-alt-text/#2-write-and-edit-the-alt-text), you might have noticed a `Generate alt text` for me button. While this feature can be convenient, we advise caution when using it. It's essential to understand that this function, in its current form, does **NOT** always produce accurate or comprehensive alt text. Nevertheless, we will guide you on how to utilize this tool and subsequently review the auto-generated alt text for accuracy.

## 1. Click the `Generate alt text for me` button.

**View Alt Text …** → Go to the Alt Text panel  → **Generate alt text for me**

## 2. Review the generated alt text.

Note that the quality of Alt Text is not guaranteed, so please do not just click that button and call it a day. If I generate the alt text automatically for the plot, it'll just show a non-descriptive text -- "Diagram", which is not informative at all.

<img src="{{site.baseurl}}/assets/images/PowerPoint/alt-text-4.png" alt='This is a screenshot of a powerpoint slide and the Alt Text Panel. On the left, there is a powerpoint slide with a scatterplot and a red line fitting a regression of the scatter plot. On the right, the auto-generated alt text is "Diagram, description automatically generated."'>

## 3. Language models and alt text generation

We recommend not using tools like GPT4 to generate alt-text. These models often produce very verbose text descriptions and may get numerical values incorrect. We highly recommend taking a very close look, and manually verifying the alt-text if a generative AI program is used to generate them. 