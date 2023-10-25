---
title: Homework Write-up Accessibility
layout: default
nav_order: 4
permalink: /docs/homework
---

# How to Make Homework Write-Up Accessible?
{: .fs-9 }

Homework write-up typically takes the form of a PDF file. Students download the PDF file, fill in the answers, and submit it to the instructor. However, PDF files are not often accessible to screen reader users. One solution is to accessible [Markdown](https://daringfireball.net/projects/markdown/syntax#philosophy) files, which is a small text-to-HTML conversion language to enable formatting text in a plain text editor.

## 1. Use Markdown or LaTeX to write your homework

Notably, Markdown is accessible to screen reader users and can be easily converted to PDF files, too. 

{: .important }
One convenient way is to **maintain a central Markdown file**, which can be converted to a PDF file using `pandoc`. The benefit is that screen readers work with PDF files, especially when combined with Mathjax for math notation:

```bash
pandoc --toc --standalone --mathjax -f markdown -t html YOUR_HOMEWORK_FOLDER/*.md -o YOUR_HTML_NAME.html --metadata title=“HOMEWORK_TITLE"
```

* [`pandoc`](https://pandoc.org/) is open-source document converter software. It is widely used for converting academic papers and technical documents to various formats, including HTML, PDF, and Microsoft Word.
* `--toc` adds a table of contents to the converted document
* `--standalone` means that the output is a standalone file 
* `--mathjax` MathJax is a JavaScript plugin that works with screen readers for math notation.
* `YOUR_HOMEWORK_FOLDER/*.md` is the homework folder that contains your markdown files.
* `YOUR_HTML_NAME.html` is the output html file. You can host this file on your course website.

{: .note }
You can follow the same process if you had used LaTeX to set up your homework. To do this, replace `markdown` with `latex`.

## 2. Example using LaTeX

Below is a running example of converting a homework folder with LaTeX files into an HTML file:

* Create LaTeX files for your homework. For example, this homework includes three questions. (`main.tex`, inside sub-folders include `association_rules.tex`, `lsh.tex`, etc.). You can create your files as you would usually do with LaTeX.

<img src="{{site.baseurl}}/assets/images/Homework/homework-1.png" alt='This is a screenshot of a directory on Google Drive. It includes 4 folders (association_rules, lsh, lsh_coding, spark) and 3 latex files (hw1_template.tex, main.tex, and policies.tex)' width="400">

* In your terminal, run the following command to compile the LaTeX files to MathJax using one simple command:

```bash
pandoc --toc --standalone --mathjax -f latex -t html YOUR_SOURCE_LATEX_FILE.tex -o YOUR_HTML_NAME.html --metadata title="HOMEWORK_TITLE" 
```

In the command, replace the `YOUR_HOMEWORK_FOLDER`, `YOUR_HTML_NAME.html`, `HOMEWORK_TITLE` with your own setup. 

* Open the `YOUR_HTML_NAME.html`. Move the HTML file to your course server. That’s it! You can find an example of the generated HTML file at this [link](https://htmlpreview.github.io/?https://github.com/rrrrrrockpang/CSE547-Accessible/blob/main/homework/homework-1/hw1.html)

Overall, this process generates an HTML file based on the Markdown or LaTeX files that you might already have. We found the generated HTML to be of acceptable quality.
