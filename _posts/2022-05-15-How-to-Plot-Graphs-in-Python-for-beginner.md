---
title: How to Plot Graphs in Python (Matplotlib)
description: This blog will introduce you guide on creating various types of graphs in Python using the Matplotlib library.
author: Cyberthirtry
date: 2022-05-15 11:33:00 +0200
categories: [Programming]
tags: [python, matplotlib, data visualization, programming, tutorial]
math: true
mermaid: true
image:
  path: /common/graph.jpg
  lqip: data:image/webp;base64,UklGRpoAAABXRUJQVlA4WAoAAAAQAAAADwAABwAAQUxQSDIAAAARL0AmbZurmr57yyIiqE8oiG0bejIYEQTgqiDA9vqnsUSI6H+oAERp2HZ65qP/VIAWAFZQOCBCAAAA8AEAnQEqEAAIAAVAfCWkAALp8sF8rgRgAP7o9FDvMCkMde9PK7euH5M1m6VWoDXf2FkP3BqV0ZYbO6NA/VFIAAAA
  alt: Matplotlib Graph
---

[![TryHackMe](https://img.shields.io/badge/TryHackMe-%23000000?logo=tryhackme&logoColor=white&style=for-the-badge)](https://tryhackme.com/p/cyber30)
[![Hack The Box](https://img.shields.io/badge/HackTheBox-%23000000?logo=hackthebox&logoColor=white&style=for-the-badge)](https://app.hackthebox.com/profile/1751803)

# How to Plot Graphs in Python (Matplotlib)

## Introduction

Data visualization is an essential aspect of data analysis and interpretation. Matplotlib is one of the most widely used libraries in Python for this purpose. In this guide, we will explore how to plot various types of graphs using Matplotlib.

## Getting Started

First, you need to install Matplotlib. You can do this using pip:

```sh
pip install matplotlib
```

Once installed, you can start using Matplotlib to create different types of plots.

## Create a plot figure

- First import matplotlib modules
- Plot the x, y coordinates & color
- Plot the graph use .show()
  
  ```python
  import matplotlib.pyplot as plt
  
  # Create the plot
  plt.plot([2, 11, 15, 40], [4, 8, 15, 22])
  
  # Add title and labels
  plt.title(' Line Plot')

  # plot the x, y con
  plt.xlabel('X-axis')
  plt.ylabel('Y-axis')
  
  # Show the plot
  plt.show()
  ```

## Scatter Plot

A scatter plot can be created as follows:

```python
import matplotlib.pyplot as plt

# Sample data
x = [1, 2, 3, 4, 5]
y = [2, 3, 5, 7, 11]

# Create the scatter plot
plt.scatter(x, y)

# Add title and labels
plt.title('Scatter Plot')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')

# Show the plot
plt.show()
```

## Bar Plot

Creating a bar plot is just as simple:

```python
import matplotlib.pyplot as plt

# Sample data
categories = ['A', 'B', 'C', 'D', 'E']
values = [5, 7, 3, 8, 4]

# Create the bar plot
plt.bar(categories, values)

# Add title and labels
plt.title('Bar Plot')
plt.xlabel('Categories')
plt.ylabel('Values')

# Show the plot
plt.show()
```

## Histogram

You can also create histograms to show the distribution of data:

```python
import matplotlib.pyplot as plt

# Sample data
data = [1, 2, 2, 3, 3, 3, 4, 4, 4, 4, 5, 5, 5, 5, 5]

# Create the histogram
plt.hist(data, bins=5, edgecolor='black')

# Add title and labels
plt.title('Histogram')
plt.xlabel('Data')
plt.ylabel('Frequency')

# Show the plot
plt.show()
```

## Pie Chart

A pie chart can be created using the following code:

```python
import matplotlib.pyplot as plt

# Sample data
labels = ['A', 'B', 'C', 'D']
sizes = [15, 30, 45, 10]

# Create the pie chart
plt.pie(sizes, labels=labels, autopct='%1.1f%%', startangle=140)

# Add title
plt.title('Pie Chart')

# Show the plot
plt.show()
```

## Summary

Matplotlib is a powerful library for creating a wide variety of graphs and plots in Python.
Happy plotting!
