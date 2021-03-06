---
layout: post
title: 10 Differentiation
---

Taking numerical derivatives is based on the elementary definition

$$
\frac{dy(t)}{dt} := \lim_{h\rightarrow 0} \frac{y(t+h) - y(t)}{h}
$$

We will then derive different finite difference approximations to the
derivative and assess their error.

## Class material

You can follow the lecture in the slides
[10-differentiation.ipynb]({{site.nbviewer.resources}}/10_differentiation/10-differentiation-part-1.ipynb).
[^1]

For the problem that you should solve during the class, get the
notebook
[10-differentiation-students.ipynb]({{site.nbviewer.resources}}/10_differentiation/10-differentiation-students.ipynb)
(`git pull` [your PHY494-resources repository]({{site.baseurl}}{%
post_url 2017-01-24-04_Git_basics %}#class-resources-on-github)).


#### Additional resources

* _Computational Physics_: Ch 5.1 -- 5.6
* If you are interested in *integration* then see
  [the lectures on integration in 2016](https://asu-compmethodsphysics-phy494.github.io/ASU-PHY494-2016/2016/02/09/07_Integration/);
  this year we are skipping this part in favor of more in-depth
  programming exercises.

--------

#### Footnotes

[^1]:

    The notebook is not complete yet ("part 1"); the full notebook
    [10-differentiation.ipynb]({{site.nbviewer.resources}}/10_differentiation/10-differentiation.ipynb)
    will be posted *after* the student exercise
    [10-differentiation-students.ipynb]({{site.nbviewer.resources}}/10_differentiation/10-differentiation-students.ipynb)
    has been completed.
