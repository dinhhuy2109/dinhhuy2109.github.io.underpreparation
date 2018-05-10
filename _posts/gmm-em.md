---
layout: post
category: blog
title: "Gaussian mixture models and the EM algorithm, python package scikit-learn"
excerpt: "A short introduction to GMM and EM algorithms, tutorials to scikit-learn."
tags: [learning, GMM, EM, sklearn, python]
comments: false
---

# What is EM, GMM? How it works?

A Gaussian mixture model (GMM) is a probabilistic model that assumes all the
data points are generated from a mixture of a finite number of
Gaussian distributions with unknown parameters. One can think of
mixture models as generalizing k-means clustering to incorporate
information about the covariance structure of the data as well as the
centers of the latent Gaussians.

A GMM is
useful for modeling data that comes from one of several groups: the
groups might be different from each other, but data points within the same group can be well-modeled by a
Gaussian distribution.

{:refdef: style="text-align: center;"}
<figure>
  <img src="{{ site.url }}/images/gmm-example.pdf">
  <figcaption>"Fig.: An example of a mixture of 2 Gaussian
  distributions"</figcaption>
</figure>
{: refdef}

Below is a collection of videos with some intuitive examples for EM,
GMM algorithms
[https://goo.gl/2up9C3](https://goo.gl/2up9C3)

In case you need more math, this
[note](https://people.csail.mit.edu/rameshvs/content/gmm-em.pdf) is
also very useful.

# Scikit 
Scikit-learn implements different classes to estimate Gaussian mixture
models, that correspond to different estimation strategies.

## Scikit Installation
For Linux and MacOS, If you already have a working installation of
numpy and scipy, the easiest way to install scikit-learn is using pip
```{bash}
pip install -U scikit-learn
```
or conda:

```{bash}
conda install scikit-learn
```
*Note: Please be consistent when using pip or conda, e.g. to upgrade
or uninstall scikit-learn installed with Anaconda or conda you should
not use the pip command.*

## Scikit.mixture examples


