---
title: Scenario 4 - Genetic Analysis on AML
---

# Scenario 4: Genetic Analysis on AML

## Cell Line Derived from a Patient with AML

A researcher is interested in the diversity and prevalence of genetic aberrations that cause AML in patients. A cell line has been derived from a patient with acute myeloid leukemia (AML). In order to acquire data that can be used for genetic analysis on this cell line, whole transcriptome RNA sequencing was performed of which the results have been used as input of the HAMLET pipeline. The HAMLET pipeline enables simultaneous detection of genetic mutations resulting in a phenopacket dataset that stores genetic as well as phenotypic information.

---

## Research Questions

### Question 1: Gene Mutation Prevalence

Have patients been observed with variants in the same gene and the same diagnosis?

To answer this question the genes are found in which at least one mutation is present given the phenopacket of the AML cell line identified as `new-reference-files` and given a set of other instances of phenopackets collected from a public data source. This database contains phenopackets holding information from different published cases and cohort reports. The next step is to acquire the diagnosed diseases with which the relevant mutations are associated in the collected phenopackets. These steps are performed in the following SPARQL query:

```{literalinclude} SPARQL/scenario_4/question1_a.rq
:language: sparql
```

From the collection of available phenopackets, a disease other than AML associated with a mutation in the same gene as for the given AML cell line is identified based on the query result shown below:

```{glue} scenario4_diagnosis
:doc: hamlet_notebook.ipynb
```

---

## Conclusion

Given the observations, patients have been found with variants in the same gene as in the AML cell line being the gene NRAS. However, these patients are diagnosed with a different disease, Noonan syndrome 6. 

---