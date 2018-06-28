---
layout: post
title: Siamese Network for Chromosome Classification
permalink: /projects/chromosomeClassification
---

Karyotyping is the process of pairing and ordering 23 pairs of human chromosomes from cell images on the basis of size, centromere position, and banding pattern. Karyotyping during metaphase is often used by clinical cytogeneticists to analyze human chromosomes for diagnostic purposes. It requires experience, domain expertise and considerable manual effort to efficiently perform karyotyping and diagnosis of various disorders. Therefore, automation or even partial automation is highly desirable to assist technicians and reduce the cognitive load necessary for karyotyping. This work attempts to develop methods for chromosome classification by borrowing the latest ideas from deep learning. More specifically, it perform straightening on chromosomes and feed them into Siamese Networks to push the embeddings of samples coming from similar labels closer. Further, it performs balanced sampling from the pairwise dataset while selecting dissimilar training pairs for Siamese Networks, and an MLP based prediction on top of the embeddings obtained from the trained Siamese Networks. The experiments were performed on a real world dataset of healthy patients collected from a hospital, followed by exhaustive comparision of the effect of different straightening techniques, by applying them to chromosome images prior to classification.

Worked with the lab-mates, under the guidence of [Dr. Lovekesh Vig](https://sites.google.com/site/lovekeshhome/). 

<iframe src="//www.slideshare.net/slideshow/embed_code/key/ecyF8hr9FSU2ZM" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen> </iframe> 

The work is published at BIC, [ICCV-2017](http://iccv2017.thecvf.com/). For details of this project refer [Paper](https://gaurav16gupta.github.io/papers/Siamese%20Networks%20For%20Chromosome%20Classification_BIC_ICCV2017.pdf).
