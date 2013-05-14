---
layout: post
title: "Explore and get public fMRI datasets from COINS Data Exchange"
date: 2013-05-14 13:29
comments: true
categories: [Datasets, Database, COINS]
---

<img src="http://d1yzvr466z4u1c.cloudfront.net/image02.jpg" alt="COINS Banner" style="width:100%;" />

COINS manages fMRI, MEG and phenotypic data for over 400 studies across six research institutions.

<!-- more -->

An ever-increasing subset of this data is being made publicly available on the COINS Data Exchange. Currently, the research community can explore and request raw MRI, fMRI and phenotypic data from several independent studies.

###Tutorial: 
A simple video-tutorial for querying can be seen on the COINS Data Exchange site, or on [YouTube](http://www.youtube.com/watch?v=YjMbCq5NBuc).

{% youtube YjMbCq5NBuc %}

###Exploration:
Creating a COINS account is easy. Just go to <http://coins.mrn.org/dx>, enter your email address, make up a password and click ‘Get Account’.  That account is needed to let you know when your data are available for download, and to track any data agreements necessary for specific datasets. It is recommended that you do this prior to the Hackathon, just to explore the Data Exchange before needing to use it.  

Once your account has been created, you can browse data in the Data Exchange. A unique filtering tool allows you to construct complex queries by combining data filters into logical groups and sub-groups. The goal of the exploration should be to target the exact data that is useful to you before you request and download it. This will save bandwidth and computing time on the COINS servers. Additionally, a well-targeted request will save you time by decreasing the need to post-filter data after download.  

###Approval:
Once you have found your ideal data, you can request that data by clicking the ‘Request’ button at the top-right. Though all data in the COINS data exchange is fully anonymized and defaced, some studies will need to explicitly approve your request. For this reason, you can provide information about your intentions for the data that you are requesting. Other studies (ABIDE, for example) have pre-approved their data for instant download. Each data-source is approved independently, so you can start downloading data as it is approved. 


###Delivery:
Approved data is packaged into ‘Data Capsules’ on the COINS servers. You will receive an email when your Data Capsule is ready, and you can then begin your download(s).


###Using COINS Data Exchange to meet your OHBM Hackathon objectives: 
At present, the COINS Data Exchange is only accessible through the browser interface at <http://coins.mrn.org/dx>. However, once your data has been approved and packaged for download, you can download each data capsule directly to another web-server or cloud-based storage device from the command line or a script. 

After choosing which capsule to download, a dialog will appear with a temporary URL that can be used to request the capsule directly. The link will expire as soon as the download button is clicked, or after five minutes, so please do not click on the data until you are ready to download it.. 
<img src="http://d1yzvr466z4u1c.cloudfront.net/image01.png" alt="COINS Banner" style="max-width:100%;" />

Downloaded imaging data may consist of DICOM or NIfTI files, and will be organized in the following file-hierarchy:

<img src="http://d1yzvr466z4u1c.cloudfront.net/image00.png" alt="COINS Banner" style="max-width:100%" />

Downloaded phenotypic (assessment) data will be contained in CSV files: one per instrument (questionnaire form). 

###Currently Available Datasets:

- __ABIDE:__ from <http://fcon_1000.projects.nitrc.org/indi/abide/>: In response, the Autism Brain Imaging Data Exchange (ABIDE) hereby provides previously collected resting state functional magnetic resonance imaging (R-fMRI) datasets from 539 individuals with ASD and 573 typical controls for the purpose of data sharing in the broader scientific community. Various cognitive and clinical assessments are also available. These data are pre-approved for sharing. 

-  __Discovery Sci:__ <http://fcon_1000.projects.nitrc.org/indi/pro/nki.html>: The NKI/Rockland Sample is intended to be a phenotypically rich neuroimaging sample, consisting of data obtained from individuals between the ages of 4 and 85 year-old. All individuals to be included in the sample undergo semi-structured diagnostic psychiatric interviews, and complete a battery of psychiatric, cognitive and behavioral assessments in order to provide comprehensive phenotypic information for the purpose of exploring brain/behavior relationships. Data from the NKI/Rockland sample will be given away prospectively, during the course of acquisition (randomized 2-8 week lag). These data require a data sharing agreement which can be quickly approved. 

- __MCIC:__ The MIND Clinical Imaging Consortium is composed of The Mental Illness and Neuroscience Discovery Institute, now the Mind Research Network (MRN, <http://mrn.org>), comprised of investigators at the University of New Mexico, the University of Minnesota, Massachusetts General Hospital, and the University of Iowa (data from this site not available). The MCIC consortium conducted a cross-sectional study to identify quantitative neuroimaging biomarkers of schizophrenia. Expertly collected, well-curated data sets consisting of comprehensive clinical characterization and raw structural, functional and diffusion-weighted DICOM images in schizophrenia patients (n=162) and sex and age-matched controls (n=169) are now accessible to the scientific community. These data also require a data sharing agreement which can be quickly approved.

###Contact:
The COINS developers are excited to support the OHBM Hackathon participants. Any requests, questions or feedback can be directed to <ni@mrn.org>.
