---
layout: post
title: "NeuroDebian: The ultimate neuroscience software platform"
date: 2013-06-11 18:00
comments: true
categories: [Virtual Machines, Operating Systems, Datasets, Atlases, Software, NeuroDebian]
---

{% img /images/NeuroDebian.png "NeuroDebian" %}

[NeuroDebian][] is a turnkey software platform for nearly all aspects of the neuroscientific research process.
It provides a large collection of popular neuroscience research software for the [Debian][] operating system as well as [Ubuntu][] and other derivatives.  Moreover it provides some popular datasets and atlases within the same convenient package management system.


<!-- more -->

### Software

Popular neuroscience-oriented packages include [AFNI][], [FSL][], [PyMVPA][] and [many others][software].  In addition popular projects for generic (e.g. [pandas](http://neuro.debian.net/pkgs/python-pandas.html), [xppaut](http://neuro.debian.net/pkgs/xppaut.html)) and distributed (e.g. [coop-computing-tools](http://neuro.debian.net/pkgs/coop-computing-tools.html), [condor](http://neuro.debian.net/pkgs/condor.html)) computation needs are included.  The [entire list][software] is too long to cite here.

### Data

- Atlases provided by software such as [FSL][] and [AFNI][]
- [NeuroSynth dataset][] and [its FSL atlas][NeuroSynth FSL atlas]
- [Haxby 2001][] dataset
- [PyMVPA tutorial][] (including data and IPython notebook)
- See [our website][data] for the exhaustive list

### Installation

Majority of software packaged by NeuroDebian team is integrated are already available on any stock [Debian][] or [Ubuntu][] system.  In addition we maintain a dedicated [NeuroDebian repository](http://neuro.debian.net/#get-neurodebian) which you could add to APT sources on your stock Debian/Ubuntu installation to obtain most recent versions and software we maintain AND data packages which are absent from official Debian and Ubuntu archives.

#### Personal virtualization

Pre-crafted [NeuroDebian virtual appliance][virtual machine] allows to start using NeuroDebian and thousands of available software packages on any operating system in matter of minutes.

#### Cloud

NeuroDebian provides software for the NITRC-CE environment available for the hackathon participants.

### Support

[Email us directly](mailto:team@neuro.debian.net) with any "private" communication.  Otherwise please use our [public mailing list][neurodebian-users] with any support questions.
You are welcome also to join #neurodebian IRC room on OFTC network if you have quick questions or want to join a live discussion.

Please visit our [support][] page for additional channels.

### Conclusion

If you are not using NeuroDebian *already* - you must try it now!

[NeuroDebian]: http://neuro.debian.net
[Debian]: http://www.debian.org
[Ubuntu]: http://www.ubuntu.com
[nitrc]: http://www.nitrc.org
[virtual machine]: http://neuro.debian.net/vm.html
[virtual machine installation instructions]: http://neuro.debian.net/vm.html#installation
[software]: http://neuro.debian.net/pkgs.html
[data]: http://neuro.debian.net/pkglists/toc_pkgs_for_release_data.html
[support]: http://neuro.debian.net/about.html#chap-contacts

<!-- some packages work mentioning -->

[AFNI]: http://neuro.debian.net/pkgs/afni.html
[FSL]: http://neuro.debian.net/pkgs/fsl.html
[PyMVPA]: http://neuro.debian.net/pkgs/python-mvpa2.html
[PyMVPA tutorial]: http://neuro.debian.net/pkgs/python-mvpa2-tutorialdata.html
[Haxby 2001]: http://neuro.debian.net/pkgs/haxby2001-faceobject.html
[NeuroSynth dataset]: http://neuro.debian.net/pkgs/neurosynth-dataset.html
[NeuroSynth FSL atlas]: http://neuro.debian.net/pkgs/fsl-neurosynth-atlas.html

[neurodebian-users]: http://lists.alioth.debian.org/mailman/listinfo/neurodebian-users
[neurodebian-devel]: http://lists.alioth.debian.org/mailman/listinfo/neurodebian-devel
[neurodebian-upstream]: http://lists.alioth.debian.org/mailman/listinfo/neurodebian-upstream
