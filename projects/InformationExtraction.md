---
layout: post
title: Information Extraction from Hand-marked Industrial Inspection Sheets
permalink: /projects/InformationExtraction
---

In order to effectively detect faults and maintain heavy machines, a standard practice in several organizations is to conduct regular manual inspections. The procedure for conducting such inspections requires marking of the damaged components on a standardized inspection sheet which is then camera scanned. These sheets are marked for different faults in corresponding machine zones using hand-drawn arrows and text. This project aims to make a novel pipeline to build an information extraction system for such machine inspection sheets, utilizing state-of-the-art deep learning and computer vision techniques. The pipeline proceeds in the following stages:

1. Localization of different zones of the machine, arrows and text using a combination of template matching, deep learning
and connected components, and 

2. Mapping the machine zone to the corresponding arrow head and the text segment to the arrow tail, followed by pairing them to get the correct damage code for each zone. 

Experiments were performed on a dataset collected from an anonymous real world manufacturing unit.

Below given flowchart depicts the proposed methodology. The first stage involves independently localizing the arrows, the text regions and the machine zones. The second stage involves mapping arrow heads to machine zones and arrow tails to text regions. The machine zones can then be directly mapped to the corresponding text regions.

<p>
<img src="/images/inspection_flow.jpg" align="center">
</p>

Refer to the presentation below for the overview of the project. For more information refer [Paper](https://gaurav16gupta.github.io/papers/cbdar.pdf)

<iframe src="//www.slideshare.net/slideshow/embed_code/key/oFWpMAhiqVOgUE" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen> </iframe> 

