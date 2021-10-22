---
layout: home
title: Empirical Foundations of Machine Learning
nav_exclude: true
seo:
  type: Autumn 2021
  name: Empirical Foundations of Machine Learning
---

# {{ site.tagline }}
{: .mb-2 }
{{ site.description }}
{: .fs-6 .fw-300 }

{% if site.announcements %}
[Announcements](announcements.md){: .btn .btn-outline .fs-3 }
{% endif %}

## About

Many advances from the past decade of machine learning are empirical in nature, but the assumptions underlying common experimental frameworks are often unclear and sometimes invalid. This course will examine machine learning from the perspective of an experimental science. We will start with fundamentals from applied statistics, learning theory, causality, and philosophy of science to build a rigorous toolkit for analyzing machine learning experiments. We will then see these concepts in action when we discuss key empirical advances from the past decade of machine learning research. The course will place a particular focus on the role of datasets, evaluations, and reliable generalization. Finally we will proceed to the research frontier in these directions and discuss recent papers, the current state of the field, and possible future developments.

Why focus on empirical foundations? Many papers in machine learning follow a common experimental framework: Researchers propose a new method, evaluate it on a dataset, and claim success if the method improves over prior baselines. While the resulting methods sometimes appear ad-hoc and without principled motivation, this approach to machine learning has still been highly influential over the past decade and produced ubiquitous methods such as ResNets or Transformers. At the same time, the existing evaluation paradigm is coming under increasing pressure from the rapid growth of machine learning and the heightened expectations users have for the resulting methods. Indeed, there is now a growing literature on reliability concerns and failed evaluations in machine learning. This course will prepare students to engage with this literature and conduct rigorous experiments in machine learning.

The class format will be a combination of lectures and discussions. The lecture part will focus on fundamentals and provide students the basic tools to (i) identify the causal structure in scientific hypotheses, (ii) design experiments to test these hypotheses, and (iii) conduct statistical analyses of these experiments (confidence intervals, bootstrap, etc.). The discussions will be centered around papers and connect the aforementioned fundamentals to contemporary machine learning. Students who take the class for credit will be expected to participate in discussions and conduct a quarter-long research project.


## Lecture

Tuesday / Thursday 10 - 11:20 am PT  CSE2 G04 (Gates building).

**Lecture 1**{: .label .label-purple }Introduction (Sept. 30, [one page per slide](/au21/assets/lectures/cs599_au21_lecture_01.pdf), [one page per animation](/au21/assets/lectures/cs599_au21_lecture_01_build.pdf)).

**Lecture 2**{: .label .label-purple }Project motivation and details (Oct. 5, [one page per slide](/au21/assets/lectures/cs599_au21_lecture_02.pdf), [one page per animation](/au21/assets/lectures/cs599_au21_lecture_02_one_page_per_animation.pdf)).

**Lecture 3**{: .label .label-purple }Additional logistics, introduction to benchmarks, and confidence intervals (Oct. 7, [one page per slide](/au21/assets/lectures/cs599_au21_lecture_03.pdf), [one page per animation](/au21/assets/lectures/cs599_au21_lecture_03_one_page_per_animation.pdf)).

[All of Statistics](https://www.springer.com/gp/book/9780387402727) by Larry Wasserman is a great general reference for statistics.

**Lecture 4**{: .label .label-purple }Statistics I (Oct. 12).

* The first part of the lecture was based on [Kevin Jamieson's](https://homes.cs.washington.edu/~jamieson/about.html) [probability review](https://courses.cs.washington.edu/courses/cse599i/18wi/resources/lecture3/lecture3.pdf) in his class on [online and adaptive machine learning](https://courses.cs.washington.edu/courses/cse599i/18wi/).
* The second part of the class followed Chapter 1 in the [high-dimensional statistics](http://www-math.mit.edu/~rigollet/PDFs/RigNotes17.pdf) lecture notes by [Philippe Rigollet](http://www-math.mit.edu/~rigollet/) and [Jan-Christian Hütter](https://www.jchuetter.com).
* The [Jupyter notebook](/au21/assets/lectures/class_4_5.ipynb) to illustrate the coverage properties of confidence intervals.

**Lecture 5**{: .label .label-purple }Discussion 1 (Oct. 14, ImageNet).

**Lecture 6**{: .label .label-purple }Statistics II (Oct. 19 , see statistics resources below).
* The treatment of sub-Gaussian random variables and their properties was based on Chapter 1 in the [high-dimensional statistics](http://www-math.mit.edu/~rigollet/PDFs/RigNotes17.pdf) lecture notes by [Philippe Rigollet](http://www-math.mit.edu/~rigollet/) and [Jan-Christian Hütter](https://www.jchuetter.com) and [Martin Wainwright's](https://people.eecs.berkeley.edu/~wainwrig/) book on [high-dimensional statistics](https://www.cambridge.org/core/books/highdimensional-statistics/8A91ECEEC38F46DAB53E9FF8757C7A4E).
* The derivation of Clopper-Pearson confidence intervals followed the [lecture notes](http://faculty.washington.edu/fscholz/DATAFILES498B2008/ConfidenceBounds.pdf) by [Fritz Scholz](http://faculty.washington.edu/fscholz/).
* The [Jupyter notebook](/au21/assets/lectures/class_4_5.ipynb) to illustrate the coverage properties of confidence intervals.
* The Python package statsmodels has [implementations](https://www.statsmodels.org/stable/generated/statsmodels.stats.proportion.proportion_confint.html?highlight=clopper) of multiple confidence intervals.

There are many more excellent resources on concentration of measure, for instance
- The book [High-Dimensional Probability](https://www.math.uci.edu/~rvershyn/papers/HDP-book/HDP-book.html) by Roman Vershynin.
- The lecture notes [Probability in High Dimension](https://web.math.princeton.edu/~rvan/APC550.pdf)  by Ramon van Handel.
- The book [Concentration Inequalities: A Nonasymptotic Theory of Independence](https://oxford.universitypressscholarship.com/view/10.1093/acprof:oso/9780199535255.001.0001/acprof-9780199535255) by Stéphane Boucheron, Gábor Lugosi, and Pascal Massart.

**Lecture 7**{: .label .label-purple }Discussion 2 (Oct. 21, AlexNet and ResNet).



## Assignments

### Course Project

Project proposals are due Tuesday, October 19 at 10am PT. 
Only one person in your group of 1-3 must submit a proposal, 
by email to Ludwig and Mitchell (please list all members on the PDF).

The proposal deadline has been extended to from October 14 to 
October 19 so that it
does not conflict with the first paper reading seminar.

The proposal should be 1-2 pages including sketches of 
the main plots (does not have to be real data), 
and describe the goals of your team for the final 
project (including details such as datasets, etc.).

### Role-Playing Paper-Reading Seminars

Inspired by [Alec Jacobson](https://www.cs.toronto.edu/~jacobson/) and 
[Colin Raffel](https://colinraffel.com/), we will be discussing papers in 
the [many-to-many role-playing format](https://colinraffel.com/blog/role-playing-seminar.html).

Roles and their descriptions can be found [here](https://colinraffel.com/blog/role-playing-seminar.html), though we will make the following modifications:
- Added role: summarizer. This team will be responsible for providing a short 8 minute summary of the papers and will be the first role to present.
- Added role: connector. This team will be responsible for connecting the two papers to each other, and to other papers we have read or discussed.
- Modified role: The scientific peer reviewer has been split into two roles, a positive reviewer (advocate) and a negative reviewer (skeptic).

Logistics will work as follows:
- At least 3 days before the discussion (i.e., Monday for a Thursday discussion) please start a group message with your team on Mattermost.
- Before the discussion, upload your slides to the shared google slides and decide on a presenter.
- All roles will have 4 minutes to present which will be followed by a 4 minute discussion, except the summarizer who will have 8.

**Discussion 1**{: .label .label-purple } (Thursday, Oct 14): Role assignments can be found in the paper discussion channel on mattermost. We will be reading:
- [ImageNet: A Large-Scale Hierarchical Image Database](https://image-net.org/static_files/papers/imagenet_cvpr09.pdf)
- [ImageNet Large Scale Visual Recognition Challenge](https://arxiv.org/abs/1409.0575)

**Discussion 2**{: .label .label-purple } (Thursday, Oct 21): Role assignments can be found in the paper discussion channel on mattermost. We will be reading:
- [ImageNet Classification with Deep Convolutional Neural Networks (AlexNet)](https://papers.nips.cc/paper/2012/file/c399862d3b9d6b76c8436e924a68c45b-Paper.pdf)
- [Deep Residual Learning for Image Recognition (ResNet)](https://arxiv.org/abs/1512.03385)

**Discussion 3**{: .label .label-purple } (Thursday, Oct 28): Role assignments can be found in the paper discussion channel on mattermost. We will be reading:
- [Deep Reinforcement Learning at the Edge of the Statistical Precipice](https://arxiv.org/abs/2108.13264)
- [With Little Power Comes Great Responsibility](https://arxiv.org/abs/2010.06595)

