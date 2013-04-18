---
layout: post
title: "The National Database for Autism Research Data Dive"
date: 2013-04-18 13:02
comments: true
categories: [Challenges, NDAR, Datasets]
---

{% img http://ndar.nih.gov/images/ndar/ndar.png "NDAR" %}
This HBM Hackathon accessible dataset is an excellent resource for finding significant relationships amongst neuroimaging, clinical, and –omics data within the National Database for Autism Research ([NDAR][ndar]).

<!-- more -->

#### Background

[NDAR][ndar] is an NIH-funded research data repository that aims to accelerate progress in autism spectrum disorders (ASD) research through data sharing, data harmonization, and the reporting of research results. NDAR is a restricted access data repository, offering a wealth of data related to human subjects research in autism.  Applying for access prior to the OHBM hack event is essential.  Additionally, it serves as a scientific community platform to multiple other research repositories, allowing for aggregation and secondary analysis of clinically captured research data.

[ndar]: http://ndar.nih.gov

#### Data and Tools

Continually updated through the contributions of primary researchers, NDAR provides authorized researchers access to contemporary relevant raw data in a relatively short amount of time after its collection.  The database currently is sharing data on __48,135 individuals__ spread over __64,335 subject / age time points__ across hundreds of clinical, omics, and imaging data structures harmonized using a common data dictionary and a common subject identifier (see [NDAR data dictionary][dictionary]).  In addition to NDAR, autism data from the Autism Genetic Research Exchange, Interactive Autism Network, the Autism Tissue Program, and the normative Pediatric MRI data repository are also available, but also require approval.

[dictionary]: http://ndar.nih.gov/ndar_data_dictionary.html

#### Details

NDAR provides simple cohort selection/filtering on a variety of scores and types of data available at <http://ndar.nih.gov/query_data.html>.  Data selected can be downloaded or pre-loaded onto an Amazon EC2 instance for evaluation using the [NITRC Computational Environment][nitrc], [NeuroDebian][neurodebian] or other available tool sets. NDAR’s rich datasets are stored in Amazon’s S3, which facilitates parallel processing and better transfer rates. 

Download packages from NDAR include a single, tab-delimited text file for each data structure received, as well as any related files (e.g. imaging or omics) and a “Create Amazon RDS database” capability scheduled for May 2013. 

[nitrc]: http://www.nitrc.org/ce-forum
[neurodebian]: http://neuro.debian.net

#### Getting Started

NDAR is a restricted access data repository.  Review what’s available for download from <http://ndar.nih.gov/query_data.html> and apply for access at <http://ndar.nih.gov/ndarpublicweb/access.html>.