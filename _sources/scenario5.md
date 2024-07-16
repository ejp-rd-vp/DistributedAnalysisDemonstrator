---
title: Scenario 5 - Genetic Analysis Case Study on NRAS gene
---

# Scenario 5: Genetic Analysis Case Study on NRAS gene

## An Undiagnosed Child with Delayed Motor Development and Generalized Dysmorphism

On clinical examination, the undiagnosed child was found to have several facial dysmorphisms, in particular a broad neck and low-set ears. It has also been assessed that the child exhibits delayed motor development.

Genetic testing has been performed using Whole Exome Sequencing (WES) which identified a probable pathogenic mutation in the NRAS gene.

---

## Research Questions

### Question 1: Gene Mutation Prevalence

Are there any other individuals with a mutation in the same gene?

To answer this question the SPARQL query below has been used for finding the phenopackets that include at least one mutation in the NRAS gene. To identify the correct gene descriptions, the HGNC gene ID is used of NRAS being [HGNC:7989](https://www.genenames.org/data/gene-symbol-report/#!/hgnc_id/7989).

```{glue} scenario5_query_q1
:doc: nras_notebook.ipynb
:language: sparql
```

As shown below, a total of fourteen phenopackets have been found including phenotypic and genetic information related to mutations in the NRAS gene. This set of phenopackets has been created by the same researcher at the same datetime based on the metadata. 

```{glue} scenario5_phenopackets
:doc: nras_notebook.ipynb
```

### Question 2: Phenotype and Disease Prevalence

What phenotypes and which diseases have been observed in these individuals and how often do they occur in this group of individuals?

The phenopackets found for the previous question can now be analysed to conclude which phenotypes and diseases occur in this group of individuals. This is done by using the following SPARQL queries for acquiring the associated phenotypes and diseases, respectively:

```{glue} scenario5_diseases
:doc: nras_notebook.ipynb
:language: sparql
```

### Question 3: Matching Phenotypes

Do the found phenotypes overlap with the observed phenotypes found in the undiagnosed child?

---