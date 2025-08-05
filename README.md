# SURUS Dataset

## Purpose

The SURUS dataset consists of 523 articles and 48,833 manual annotations of 25 contextually different medical entities in unstructured scientific text. An illustration of the dataset structure is listed in the "data/images" folder. The ultimate purpose of the dataset is to identify and extract elements of PICOS (Population, Intervention, Comparison, Outcome & Study design) to help systematic literature reviewers in their task of selection of eligible literature. After fine-tuning a PubMedBERT model using in-domain records, weighed mean F1 was 0.95. More details on the setup, performance evaluation and utility of SURUS is described [here](https://bmcmedresmethodol.biomedcentral.com/articles/10.1186/s12874-025-02624-z).

## Structure

This repository contains the SURUS dataset. The dataset consists of 3 sets of records - "Indomain", "Indication out-of-domain" and "Study type out-of-domain", consisting of 400, 90 and 33 records, respectively. The evaluation setup targets the Indomain dataset for fine-tuning.

## Annotation methodology

For expansion of the dataset, the annotation methodology is included in the repository ("data" folder), describing the rules and logic behind annotation of medical entities. This way, SURUS can be internally adapted to fit the medical domain it's applied to. An example of a fully annotated scientific abstract is given in "data/images" folder.
