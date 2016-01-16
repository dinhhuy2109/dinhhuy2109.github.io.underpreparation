---
layout: page
title: Publications
excerpt: "My publications"
comments: false
---

In Colombia people are given two family names, one from each parent. That's why my publications are signed as Francisco Suárez-Ruiz.

You can also browse my <a href="http://scholar.google.es/citations?user=uXo_Q_IAAAAJ" target="_blank">Google Scholar profile</a>.


### Journal articles

{% bibliography --query @article --file publications %}

### Conference proceedings 

{% bibliography --query @inproceedings --file publications %}

### Book chapters

{% bibliography --query @incollection --file publications %}

### Theses

{% bibliography --query @phdthesis,@mastersthesis,@bachelorsthesis --file publications %}

### Patents

{% bibliography --query @patent --file publications %}

### Research reports

{% bibliography --query @techreport --file publications %}

### Websites

{% bibliography --query @online --file publications %}
