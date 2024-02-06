---
layout: post
title:  "Guide for using Jekyll"
date:   2024-02-01 11:48:46 +0200
author: Dan Näsman
categories: jekyll update
---

{% include mathjax.html %}

# Creating a new post

A new post is created by adding a new markdown file to `_posts` directory on your local branch and by pushing the newly made changes onto the remote `main` branch. This file works as a template. Make sure to add the line
```
{% raw %}{% include mathjax.html %}{% endraw %}
```
to your markdown file. The line is important for LaTex rendering.


# LaTex rendering

The following LaTex

$$
\begin{equation}
F(x)=\int f(x)dx
\end{equation}
$$

was created with

```
$$
\begin{equation}
F(x)=\int f(x)dx
\end{equation}
$$
```

For inline LaTex use `$...$`.

# Code snippets

To display code snippet use
````
```<desired programming language>
<insert code here (can be multiple lines)>
```
````

Example Python snippet
```python
def main():
	print("Hello world!")
```

# More resources

To make figures, tables, etc. check [this markdown cheat sheet](https://www.markdownguide.org/cheat-sheet/).
