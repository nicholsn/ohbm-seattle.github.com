---
layout: post
title: "OpenfMRI Now an HBM Hackathon Resource"
date: 2013-04-22 14:28
comments: true
categories: [Datasets, Challenges]
---

{% img https://openfmri.org/sites/all/themes/openfmri/logo.png height=150 "OpenfMRI" %}

The [OpenfMRI](http://openfmri.org) project provides raw and processed task fMRI datasets for use in re-analysis and mega-analysis that are now Cloud accessible.

<!-- more -->

#### Background

Currently the OpenfMRI database contains data from 18 studies (totaling 374 scanning sessions) across a wide range of different cognitive task domains, including: visual perception (object recognition, mirror reading), language processing (semantic judgments, rhyme judgments, pseudoword reading), working memory (tone counting, 1-back), cognitive control (stop signal, flanker, and Simon tasks), learning (category learning), decision making (gambling task, balloon analog risk task), memory encoding emotion regulation (reappraisal task), and social perception (false belief task).

More details about these datasets can be obtained from <http://openfmri.org/data-sets>. The data will also be made available via AWS.

#### Processing

The data have been preprocessed and analyzed through a full group-level fMRI analysis, using an automated FSL/Freesurfer-based processing stream developed specifically for this project.  The code for this analysis stream is available at <https://github.com/poldrack/openfmri>.  In addition, a nipype pipeline for this dataset has been developed by Satra Ghosh and is available at <http://www.mit.edu/~satra/nipype-nightly/users/examples/fmri_openfmri.html>. 
 
#### Example Responses to Challenges

__Challenge #1:__ Examine whether different task-relevant networks related to patterns of gene expression in the [Allen Human Brain Atlas](http://human.brain-map.org).

__Challenge #2:__ Integrate the resting state data with task data from the OpenfMRI database to identify the overlap and distinction between resting state networks and task-based networks.