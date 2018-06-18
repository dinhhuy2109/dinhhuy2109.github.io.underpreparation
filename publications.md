---
layout: page
title: Publications
excerpt: "My publications"
comments: false
---


### Journal articles

{% bibliography --query @article --file publications %}

<!-- ### Conference proceedings  -->

<!-- {% bibliography --query @inproceedings --file publications %} -->

<!-- ### Book chapters -->

<!-- {% bibliography --query @incollection --file publications %} -->

### Theses

{% bibliography --query @phdthesis,@mastersthesis,@bachelorthesis --file publications %}

<!-- ### Patents -->

<!-- {% bibliography --query @patent --file publications %} -->

### Research reports

{% bibliography --query @techreport --file publications %}

<!-- ### Websites -->

<!-- {% bibliography --query @online --file publications %} -->

### In preparation
{% bibliography --query @inpreparation --file publications %}
