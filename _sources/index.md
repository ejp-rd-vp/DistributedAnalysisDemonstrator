# Welcome to the EJP-RD FDP Infrastructure and VP Portal Demonstrator

This is a small sample book that acts as a demonstrator for the EJP-RD FDP infrastructure and related VP Portal. In this first edition, we have included three scenarios, each one with a different genetic case study. The scenarios are based on real cases and the research questions are designed to:

- Explore the relationship between the gene mutation and the observed disease
- Identify other individuals with the mutation or allelic variant
- Determine their phenotype and prognosis
- Investigate the variant frequency across different populations

## Scenarios

| Scenario | Context | Questions |
|----------|---------|-----------|
| **1** | An undiagnosed child with mental retardation and facial dysmorphisms with a negative array-CGH analysis underwent WES, which disclosed a de novo, likely pathogenic, rare variant in FBX011 gene. | <ol><li>Is there a relationship between the gene mutation and disease?</li><li>Are there any other individuals with the same mutation or allelic variant?</li><li>If there are, what is their phenotype? What can be derived from them for the prognosis?</li><li>What is the variant frequency across different populations?</li></ol> |
| **2** | A girl was diagnosed affected by a Noonan-like syndrome, but she was negative after analysis of an extended panel for Rasopathies. Following WES, a de novo likely pathogenic mutation was found in MAPK1 gene. | <ol><li>Are there any other individuals with the same mutation or allelic variant?</li><li>What is their phenotype and natural history of the disease?</li><li>What is the variant frequency across different populations?</li></ol> |
| **3** | A patient affected by spondylometaphyseal dysplasia with corner fractures, a rare form of AD osteocondrodysplasia of unknown genetic origin underwent WES analysis, which disclosed a de novo likely pathogenic mutation in FN1, a gene previously associated with glomerulopathy with fibronectin deposits, a rare kidney disease (KD) not present in the patient. | <ol><li>Are there any other individuals with the same mutation or allelic variant?</li><li>What is their phenotype?</li><li>Is it possible to establish any genotype-phenotype correlation?</li><li>What is the variant frequency across different populations?</li></ol> |

The scenarios were taken from the "Beyond One Million Genomes" project, which stated these use cases in their [Rare Disease Use Case List](https://zenodo.org/records/6139231).

## Next Steps

In the following chapters, we will present the SPARQL queries which could be used to answer the research questions for each scenario. Currently, these queries are primarily for inspiration and are not yet fully functional. They can be used to guide the development of the linked data infrastructure and the FAIR data points.

In this demonstrator, we use [CARE-SM](https://github.com/CARE-SM/CARE-Semantic-Model) as the core concept space to drive the example SPARQL queries provided here. Future editions of this demonstrator will consider other semantic models and ontologies.

```{tableofcontents}

