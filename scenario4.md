---
title: Scenario 4 - Genetic Analysis on AML
---

# Scenario 4: Genetic Analysis on AML.

## Cell Line Derived from a Patient with AML

A researcher is interested in the diversity and prevalence of genetic aberrations that cause AML in patients. A cell line has been derived from a patient with acute myeloid leukemia (AML). In order to acquire data that can be used for genetic analysis on this cell line, whole transcriptome RNA sequencing was performed of which the results have been used as input of the HAMLET pipeline. The HAMLET pipeline enables simultaneous detection of genetic mutations resulting in a phenopacket dataset that stores genetic as well as phenotypic information.

---

## Research Questions

### Question 1: Gene Mutation Prevalence

Have patients been observed with variants in the same gene and the same symptoms?

To answer this question, first the genes are found in which at least one mutation is present given the phenopacket of the AML cell line:

```{literalinclude} SPARQL/scenario_4/question1_a.rq
:language: sparql
```

```{glue} scenario4_genes
:doc: hamlet_notebook.ipynb
```

---