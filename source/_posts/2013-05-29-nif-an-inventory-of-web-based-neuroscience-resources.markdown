---
layout: post
title: "NIF: an inventory of Web-based neuroscience resources"
date: 2013-05-29 14:03
comments: true
categories: [Databases, Datasets, NIF]
---

{% img http://www.neuinfo.org/images/nif-logo.png 75 "NIF" %}

The [Neuroscience Information Framework][nif]: neuroscience data, materials, and tools  via any computer connected to the Internet.

[nif]: http://www.neuinfo.org

<!-- more -->

#### Background

Currently NIF Offers:

1. A [search][search] portal for researchers looking for neuroscience information, tools, data or materials
2. Access to content normally not indexed by search engines (i.e, the "hidden web")
3. [Tools][tools] for promoting interoperability among databases
4. The [NIFSTD ontology][ontology] covering the major domains of neuroscience (e.g., brain anatomy, cells, organisms, diseases, techniques)
5. [Developer resources][resources] for accessing the NIF vocabulary and NIF tools, such as [web services][services] and including a [tutorial][tutorial]


[search]: http://www.neuinfo.org/nif/nifgwt.html
[tools]: http://neuinfo.org/nif_components/disco/interoperation.shtm
[ontology]: http://www.neuinfo.org/vocabularies/index.shtm
[resources]: http://www.neuinfo.org/developers/index.shtm
[services]: http://neuinfo.org/developers/nif_web_services.shtm
[tutorial]: http://neuinfo.org/tutorials/developers_tool/federated_data.shtm

Some particular data sets which can be offered are Brain Connectivity Data (50316 records), Brain Activation Foci (5,145), Diseases (1,521), Microarray (642,995):

- [Integrated Nervous System Connectivity View][nervous] is an aggregated dataset of connectivity statements from BAMS, CoCoMac, BrainMaps, Connectome Wiki, the Hippocampal-Parahippocampal Table of Temporal-Lobe.com and the Avian Brain Circuitry Database.
- [Integrated Disease View][disease] is a virtual database currently indexing authoritative information on disease and treatment options from: NINDS Disorder List and PubMed Health. 
- [Activation Foci][foci] data provides functional activation foci data from published neuroimaging studies.

[nervous]: https://www.neuinfo.org/mynif/search.php?q=connectivity&first=true&cf=Connectivity
[disease]: https://www.neuinfo.org/mynif/search.php?q=connectivity&first=true&cf=Disease&t=indexable&nif=nlx_86401-1
[foci]: https://www.neuinfo.org/mynif/search.php?q=connectivity&first=true&cf=Brain%20Activation%20Foci

#### Example Responses to Challenges

__Challenge 1:__

- Use NIF neuron registry to identify cell systems in various neurodegenerative diseases and map it to ABA data.
- For different diseases, use NeuronRegistry-NeuroLex to infer from genes what specific cell populations differently effect neuron types. Also, we'd like to link those cell systems in Neurodegenerative diseases to neurotransmitter data in NeuronRegistry.
- For example, in Alzheimer we want to examine ABA genes and how differently they affect different group of neurons found in NeuronRegistry. Infer what cell populations impacted in various brain regions.
- ABA has mapped neurotransmitter related genes, thus one challenge is: __Are there specific neurotransmitter systems affected in mental disorders and do they map to any known cell type?__

__Challenge 2:__

Use NIF cell data as a bridge between resting data and projections of know cell types in various brain regions (ABA). Use Neurolex (NIF) and tractography (NIF) data we can estimate what type of cells where can cell body are and where axon projected.
