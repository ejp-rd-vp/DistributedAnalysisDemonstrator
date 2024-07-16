---
title: Scenario 4 - Genetic Analysis on AML
---

# Scenario 4: Genetic Analysis on AML

## Cell Line Derived from a Patient with AML

A researcher is interested in the diversity and prevalence of genetic aberrations that cause AML in patients. A cell line has been derived from a patient with acute myeloid leukemia (AML). In order to acquire data that can be used for genetic analysis on this cell line, whole transcriptome RNA sequencing was performed of which the results have been used as input of the HAMLET pipeline. The HAMLET pipeline enables simultaneous detection of genetic mutations resulting in a phenopacket dataset that stores genetic as well as phenotypic information.

---

## Research Questions

### Question 1: Gene Mutation Prevalence

Have patients been observed with variants in the same gene and the same symptoms?

To answer this question the genes are found in which at least one mutation is present given the phenopacket of the AML cell line and given a collected set of other instances of phenopackets. The next step is to acquire the diagnosed diseases with which the relevant mutations are associated. These steps are performed in the following SPARQL query:

```{literalinclude} SPARQL/scenario_4/question1_a.rq
:language: sparql
```

From the collection of available phenopackets, a disease other than AML is identified that is associated with a mutation in the same gene as for the given AML cell line based on the query result shown below:

```{glue} scenario4_diagnosis
:doc: hamlet_notebook.ipynb
```



---