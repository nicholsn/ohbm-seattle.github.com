---
layout: post
title: "Contest Winners Announced!"
date: 2013-06-25 17:39
comments: true
categories: [Hackathon, Contest] 
---

{% img /images/hackathon-banner.png %}

Congratulations to the winners of the HBM Hackathon Competition!

**Challenge 1:** No Sound Consensus  
**Challenge 2:** SCI  
**Challenge 3:** MindBoggle-102  

<!-- more -->

The winners of the HBM Hackathon Contest brought together multi-disciplinary teams to deliver excellent responses to the three challenges. Below is a list of the winning teams and their members for each category along with the submitted abstracts, presentations, and demo links. Join me in congratulating our winners and enjoy!

### Challenge 1. Best imaging and gene expression relationship discovered via integration of imaging data with the Allen Human Brain Atlas.

**Team "No Sound Consensus"** - Rhodri Cusack, Mark Daley, Charlotte Herzmann, Annika Linke, Jonathan Peelle, Conor Wild, Leire Zubiaurre-Elorza

- **[Presentation Link][nsc]**
- **[Visualization Demo](http://www.cusacklab.org/nsc)**
- **Abstract:**

> There is little consensus on the parcellation of human auditory cortex, especially in regards to auditory-related or auditory association areas beyond primary auditory cortex; in contrast, there is substantial agreement on the functional parcellation of visual cortex. This might be because: fewer scientists study the auditory system and the key analyses are still lacking; auditory regions are smaller and/or too variable across individuals; or because the auditory system is fundamentally less modular, perhaps because the statistics of environmental sounds are such that processing is best implemented in a distributed monolithic system. Our hackathon project had two overarching goals:  (1) to quantify modularity in auditory and visual systems; and (2) if appropriate, to derive a parcellation of the auditory system. As any single type of data is subject to biases, three types were brought together by an international and multidisciplinary team of scientists using multiple packages and programming languages. We first defined broad auditory and visual seed regions of interest using an open-source meta-analytic approach (i.e., http://neurosynth.org/) combined with anatomical masking. We then characterized the signature of connectivity of each voxel in these seed regions using diffusion and resting state data provided by the Human Connectome Project. Graph theory analyses were then applied to derive clusters of voxels (i.e., modules) that exhibited similar patterns of anatomical and functional connectivity, and to compare the modularity of auditory and visual cortices. Modularity of auditory cortex was found to be similar to that of visual cortex, suggesting that across individuals this system appears to have multiple distinct sub-regions. Parcellations in all seed regions showed consistency across individuals and modalities, and allowed us to derive group and grand (i.e., multi-modal) parcellations. Finally, using the Allen Brain Atlas we found that gene expression was more similar within our parcellations for visual -- but not auditory --  cortex. In summary, auditory cortex was found to be modular and to show consistency across individuals, so that reliable group parcellations were be derived. Finally, we developed a web tool that can be used to browse our parcellations and the connectivity of each module. We estimate that our entry has used around 1 year’s worth of processing time of the fastest processing cores in the Amazon cloud, and that much of team was sleep deprived for the last month.

### Challenge 2. Best neural systems model or visualization based on large-scale integration of resting state fMRI data with other HBM Hackathon accessible datasets.

**Team "SCI"** - Miriah Meyer, Tom Fletcher, Sam Gerber, Sean McKenna, Wei Liu, Brandon Zielinski, Kris Zygmunt

- **[Presentation Link][sci]**
- **Abstract:**

> I will be presenting a tool that enables the visualization and exploration of the gene expression data in both the correlation space and MNI space.  By navigating and visualizing in both spaces concurrently, the gene expression data can be explored and understood more completely, helping to generate hypotheses for further testing.

### Challenge 3. MNI Mash-up: Most innovative map or aggregation of information in the MNI 152 standard.

**Team "MindBoggle-102"** - Arno Klein, Jason Tourvillle, Jay Bohland, Rich Stoner

- **[Presentation Link][mb]**
- **[Visualization Demo](http://bit.ly/12e5ftp)**
- **Abstract:**

>- Provide anatomical labels, sulcal features, and shape information for 101 brains in MNI152 space.
>- Manually label, extract features, and analyze the shape of the cortex of an Allen human brain.
>- Create a browser-based application to display region-specific gene expression data.

>Mash-up components:

>1. Allen Human Brain T1 image and gene expression data
>2. DKT cortical labeling protocol
>3. Mindboggle-101 set of brains manually labeled with the DKT protocol
>4. Mindboggle software for feature extraction, identification, and shape analysis
>5. Web framework for visualization
>6. MNI152 template

>Yesterday, we extracted and computed shape measures on all 101 brains in the Mindboggle-101 data set, and are doing the same for the Allen brain right now. Today, we propose to manually label the Allen brain using the DKT protocol and create a browser-based application to enable a user to select a labeled region in the Allen brain and display gene expression data for that region.

### Congratulations! 


[nsc]: /images/no_sound_consensus_thursday_10mins.pdf
[sci]: /images/iCorrPlot.pdf
[mb]: /images/HBM2013_Hackathon_Mindboggle102Team.pdf