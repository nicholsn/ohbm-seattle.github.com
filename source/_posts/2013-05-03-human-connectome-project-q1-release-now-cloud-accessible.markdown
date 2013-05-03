---
layout: post
title: "Human Connectome Project Q1 Release: Now Cloud Accessible"
date: 2013-05-03 13:00
comments: true
categories: Datasets
---

{% img http://www.humanconnectome.org/img/header-bg.png "Human Connectom Project" %}

The [first full quarterly HCP Data release][data] is now Cloud accessible for participants who have [registered][hcpreg] and agreed to the [Open Access Data Use Terms][hcpterms].

<!-- more -->

HBM Hackathon participants will have the opportunity for high speed access to the first full quarterly HCP Data release via Amazon Web Services. All data available from the HCP Connectome-in-a-Box can now be downloaded directly from S3, Amazon’s Simple Storage Service. 

#### This post is organized into three sections:
1. Description of the HCP Q1 Release
2. Getting Authorized to Access the HCP Data
3. Accessing HCP Data on AWS

### Description of the HCP Q1 Release 
The Q1 data release consists of multimodal MRI data collected from 68 healthy young adults who were scanned in the fall of 2012. These include all 12 subjects from our Initial Data Release. All 3T MRI scan data is included: Structural, Functional (resting state and task) and Diffusion. Behavioral data collected on all subjects is also included, with the exception of sensitive restricted-access data. Please see the [Full Release Documentation][hcpdocs] for further details.

### Getting Authorized to Access the HCP Data
There are a few steps you will need to take to get authorization to access the HCP data hosted on AWS.

#### You need to:
1. Complete the __[HCP Registration][hcpreg]__ and agree to the __[HCP Open Access Data Use Terms][hcpterms]__
2. Complete the __[HBM Hackathon Registration][hbmreg]__
3. Create an __[Amazon Web Services Account][awsreg]__
4. Email __<hbm.hackathon@gmail.com>__ with your HCP and AWS email address(es)

#### A foreword from David van Essen:
> __For distribution to all investigators interested in using HCP Connectome-in-a-Box data.__  
</br>
> __IMPORTANT NOTICE to investigators wanting to use HCP datasets available on Connectome-in-a-Box hard drives.__  
</br>
> HCP’s Connectome-in-a-Box provides imaging data from the Open Access dataset. Before using any of these data for research, you and all other investigators using the data are required to [register][hcpreg] and agree to the [Open Access Data Use Terms][hcpterms]. __This includes agreeing to comply with institutional rules and regulations__.  This may mean that you need your research to be approved or declared exempt by a committee that oversees research on human subjects (e.g., your IRB or Ethics Committee).  The released HCP data are not considered de-identified, insofar as certain combinations of HCP Restricted Data (available through a separate process) might allow identification of individuals.  Different committees operate under different national, state and local laws and may interpret regulations differently, so it is important to ask about this. If needed and upon request, the HCP will provide a certificate stating that you have accepted the HCP Open Access Data Use Terms.  
</br>
> Sincerely,  
> David C. Van Essen (PI), for the WU-Minn HCP Consortium  
> May 1, 2013  

### Accessing HCP Data on AWS
Amazon Web Services is hosting the HCP Q1 Data Release as part of its Public Data Sets on AWS program, which will enable HBM Hackathon participants to get rapid access to the HCP data. Since the data is hosted on S3 in an uncompressed format, participants can download data in parallel using tools like [s3cmd-modification][s3cmd]. 

You can use tools like [s3cmd][s3cmd] to list the contents of a directory on S3, get individual files or sync full directories. You will also be able to download directly to your personal/work computer or to a machine on the EC2 Cloud like the [NITRC Computational Environment][nitrc].

#### Getting Credentials
Ready to start downloading? Make sure you've completed the [HCP registration][hcpreg] and [created an account with AWS][awsreg].

Next, send an email to __<hbm.hackathon@gmail.com>__ with your HCP and AWS email address(es). 

We will use your HCP and AWS email address(es) to:

1. verify that you have agreed to the [Open Access Data Use Agreement][hcpterms]
2. grant you access to the HCP data on AWS.

Once verified, you will receive an email confirming that you have access to the HCP data on AWS.

#### Configuring your system
To access the data you'll want to install [s3cmd-modification][s3cmd], which will enable you to explore the [HCP Data Directory][hcpdatadir] on Amazon and will allow rapid parallel downloading ([s3cmd-modification install instructions][s3cmdinstall]).

After you install s3cmd, you need to configure it with your AWS public and secret keys, located in [AWS Security Credentials][awscreds].

    :~ s3cmd --configure
    Enter new values or accept defaults in brackets with Enter.
    Refer to user manual for detailed description of all options.

    Access key and Secret key are your identifiers for Amazon S3
    Access Key []: <your-access-key>
    Secret Key []: <your-secret-key>
    ...	

Take s3cmd out for a test drive...

List subject directories:

    :~ s3cmd ls s3://hcp.aws.amazon.com/q1/
    
    DIR   s3://hcp.aws.amazon.com/q1/100307/
    DIR   s3://hcp.aws.amazon.com/q1/103515/
    DIR   s3://hcp.aws.amazon.com/q1/111312/
    ...
    DIR   s3://hcp.aws.amazon.com/q1/937160/
    2013-04-17 06:57         0   s3://hcp.aws.amazon.com/q1/

Get a directory in parallel:

    :~ s3cmd --parallel --workers=16 get --recursive s3://hcp.aws.amazon.com/q1/100307/T1w T1w
    
    File s3://hcp.aws.amazon.com/q1/100307/T1w/BiasField_acpc_dc.nii.gz started [2 of 52]
    File s3://hcp.aws.amazon.com/q1/100307/T1w/Native/100307.L.MyelinMap.native.func.gii started [3 of 52]
    ...
    File s3://hcp.aws.amazon.com/q1/100307/T1w/T2w_acpc_dc_restore.nii.gz saved as 'T1w/T1w/T2w_acpc_dc_restore.nii.gz' (67855816 bytes in 143.3 seconds, 462.31 kB/s)
    File s3://hcp.aws.amazon.com/q1/100307/T1w/BiasField_acpc_dc.nii.gz saved as 'T1w/T1w/BiasField_acpc_dc.nii.gz' (65076318 bytes in 180.3 seconds, 352.50 kB/s)

If everything checks out, you are ready to get hacking!

[data]: http://www.humanconnectome.org/data/
[hcpreg]: http://www.humanconnectome.org/data/data-use-terms/index.html
[hcpterms]: http://www.humanconnectome.org/data/data-use-terms/open-access.html
[hcpdocs]: http://www.humanconnectome.org/documentation/Q1/
[hbmreg]: http://www.humanbrainmapping.org/hackathon
[awsreg]: http://aws.amazon.com/
[s3cmd]: https://github.com/pcorliss/s3cmd-modification
[nitrc]: https://aws.amazon.com/marketplace/pp/B00AW0MBLO
[hcpdatadir]: http://humanconnectome.org/documentation/data-release/Q1_Release_Appendix_III.pdf
[s3cmdinstall]: https://github.com/pcorliss/s3cmd-modification/blob/master/INSTALL
[awscreds]: https://portal.aws.amazon.com/gp/aws/securityCredentials


