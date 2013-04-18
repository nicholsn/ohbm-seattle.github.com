---
layout: post
title: "LONI Pipeline in the Cloud"
date: 2013-04-18 14:30
comments: true
categories: [Virtual Machines, Workflow Tools, Datasets]
---

{% img http://pipeline.loni.ucla.edu/wp-content/themes/pipeline2012/images/explore_Coin.jpg "LONI Pipeline" %}
The [LONI Pipeline][loni] is available on the Cloud as an [Amazon EC2 Instance][ec2] (i.e., virtual machine).

<!-- more -->

 Both free and paid AWS/EC2 subscriptions can be used to launch the DPS (Distributed Pipeline Server) on EC2, and click Launch Instance. Then remote clients can connect to the hostname of that instance (e.g., ec2-184-73-1-1.compute-1.amazonaws.com). After connecting to the server, you can open a workflow under Server Library and run. The Pipeline library includes 100’s of imaging and genetics software suites, atomic processing tools, datasets and resources.  For additional details on LONI Pipeline, please see <http://pipeline.loni.ucla.edu>.

[loni]: http://pipeline.loni.ucla.edu "LONI Pipeline"

[ec2]: http://pipeline.loni.ucla.edu/products-services/pipeline-server-on-ec2 "Pipeline on EC2"