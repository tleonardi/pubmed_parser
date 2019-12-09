---
title: 'Pubmed Parser: A Python Parser for PubMed Open-Access XML Subset and MEDLINE
  XML Dataset'
authors:
- affiliation: 1
  name: Titipat Achakulvisut
- affiliation: 2
  name: Daniel E. Acuna
- affiliation: 3
  name: Ted Cybulski
- affiliation: 4
  name: Kevin Henner
- affiliation: 1
  name: Konrad Kording
date: "15 December 2019"
output: pdf_document
bibliography: paper.bib
tags:
- Python
- MEDLINE
- PubMed
- Biomedical corpus
- Natural Language Processing
affiliations:
- index: 1
  name: University of Pennsylvania
- index: 2
  name: Syracuse University
- index: 3
  name: Northwestern University
- index: 4
  name: University of Washington
---

# Summary

Biomedical publications are increasing exponetially every year. If we had the ability to access, manipulate, and link this information, we could extract knowledge that is perhaps hidden within the figures, text, and citations. In particular, the repositories made avilable by [PubMed](https://pubmed.ncbi.nlm.nih.gov/) and [MEDLINE](https://www.nlm.nih.gov/bsd/medline.html) database enable these kinds of applications at an unprecendented level. Examples of applications that can be built from this dataset range from predicting novel drug-drug interactions, classifying biomedical text data, searching specific oncological profiles, disambiguating author names, or automaticly learning a biomedical ontology. Here, we propose `pubmed_parser`, which is a software to mine Pubmed and MEDLINE efficiently. `pubmed_parser` is built on top Python and can therefore be integrated into a myriad of tools for machine learning such as `scikit-learn` and deep learning such as `tensorflow` and `pytorch`.

Pubmed Parser can parse multiple Pubmed MEDLINE data derivatives such as MEDLINE XML data, references from PubMed Open Access XML dataset, figure captions, paragraphs, and more. A core part of the package, parsing XML and HTML with Pubmed Parser is extremely fast, producting either dictionaries or JSON files that can easily be part of downstream pipelines. Moreover, the implemented functions can be scaled easily as part of other MapReduce-like infrastructure such as [PySpark](https://spark.apache.org/). This allows users to parse the most recently available corpus and customize the parsing to their needs.

Pubmed Parser has already been used in published work including [@achakulvisut2019claim; @vseva2019vist; @miller2017automated; @shahri2019propheno; @galea2018sub; @abdeddaim2018mesh; @rakhi2018data; @nikolov2018data; @mesbah2018smartpub; @neves2019evaluation; @tang2019parallel]. It is also been used in multiple biomedical and natural language class projects and blog posts.

# Acknowledgements

Titipat Achakulvisut was supportyed by the Royal Thai Government Scholarship grant #50AC002. Daniel E. Acuna is supported by National Science Foundation #1800956.

# References