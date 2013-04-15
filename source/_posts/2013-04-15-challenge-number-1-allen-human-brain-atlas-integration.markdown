---
layout: post
title: "Challenge #1: Allen Human Brain Atlas Integration"
date: 2013-04-15 12:00
comments: true
categories: [Challenges, Allen Institute]
published: true
---

{% img http://www.alleninstitute.org/Assets/images/common/logo_institute.png "Allen Institute for Brain Science" %}
For this challenge, you will try to identify the best relationship between 
imaging data and gene expression data in the Allen Human Brain Atlas.

<!-- more -->

#### Background

The goal of the Allen Human Brain Atlas is to create a comprehensive map of 
transcript usage across the entire adult brain, with the emphasis on anatomically complete coverage in a small number of high-quality, clinically unremarkable brains profiled with DNA microarrays for quantitative gene-level transcriptome coverage. Further, structural brain imaging data were obtained from each individual to visualize gene expression data in its native 3D anatomical coordinate space, and to allow correlations between imaging and transcriptome modalities.

#### Data and Tools

The Atlas consists of microarray profiles of 3702 neuroanatomically precise 
subdivisions sampled over six individuals (5 males, 1 female). Each gene 
expression profile contains information for over 58,000 gene probes with 
93% of known genes represented by at least 2 probes. Sample locations were 
mapped back into the native brain MRI coordinates and subsequently to Montreal Neurological Institute (MNI) coordinate space.

These data are freely accessible via the Allen Brain Atlas data portal ([http://human.brain-map.org][brainmap]).  They have also been mirrored using Amazon's AWS S3 cloud storage [here][aws].

Use the online tools to visualize the expression data as heatmaps or projected into 3D anatomical context. An integrated data service allows users to perform differential and correlative searches to discover genes of interest.

For more detail, start with a [guided overview][overview] or see the recent [publication][pub] in Nature.

[brainmap]: http://human.brain-map.org
[overview]: http://www.brain-map.org/tutorials/index
[pub]: http://www.nature.com/nature/journal/v489/n7416/full/nature11405.html
[aws]: https://s3.amazonaws.com/Human-Brain-Atlas/index.html

#### Details

The data is divided into separate .zip files each of the 6 donors. The zip file contains:

* SampleAnnot.csv: describes every microarray sample. Structures and MNI coordinates are here.
* MicroarrayExpression.csv: normalized expression values for all samples and probes.
* Probes.csv: description of the probes and their genes.
* Ontology.csv: all structures in the hierarchical ontology. The 'structure\_id\_path' column describes the parent-child relationship.
* Contents.txt: a more detailed description of the .zip contents.

#### Getting Started

We're looking for the best relationship between gene expression in the Atlas and imaging data set. You are not restricted to any particular imaging data set.

This [sample Matlab code][matex] that might be a good place to start. It takes one of the example data sets from the Statistical Parametric Mapping (SPM) package, samples the image at all of the microarray sample MNI coordinates, and correlates the sampled values to gene expression values.

You can also look at this [sample Python code][pyex]. It uses numpy to correlate the gene expression values of all of the samples to each other for one donor. There is also some code for picking one probe per gene. It chooses the probe that is most correlated to the other probes for that gene.

For inspiration, consider reading this study that integrates imaging and gene expression data:

Mueller K, Sacher J, Arelin K, Holiga S, Kratzsch J, et al. [Overweight and obesity are associated with neuronal injury in the human cerebellum and hippocampus in young adults: a combined MRI, serum marker and gene expression study.][study] Transl Psychiatry 2: e200. doi:10.1038/tp.2012.121.

[study]: http://www.ncbi.nlm.nih.gov/pmc/articles/PMC3565188/

Good luck!

[matex]: http://api.brain-map.org/examples/spm/index.html
[pyex]: https://github.com/AllenBrainAtlas/human-analysis-examples
