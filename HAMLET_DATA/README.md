# HAMLET Analysis Data

This folder contains dummy data depicting the results of a Human AML Expedited Transcriptomics (HAMLET) pipeline run. The HAMLET pipeline enables the simultaneous detection of fusion genes, small variants, tandem duplications and gene expression and collects all information into an output file [1]. The detection of these variants focuses on a set of 13 genes in which mutations are commonly found in acute myeloid leukemia (AML). For the demonstrator in this repository, only the information is included in the RDF phenopackets related to small variants.

## From HAMLET output to phenopacket RDF 2.0

The HAMLET pipeline outputs a JSON file containing all information found by the diagnostic assays. The data does not yet conform to the phenopacket data model and therefore needs to be converted in order to align to this data structure. To achieve this, a workflow has been developed that, given a JSON file containing the information required to form a phenopacket, generates RDF data that complies to the RDF data model schema of phenopackets version 2.0. This schema is expressed using Shape Expressions (SheX) which can be found [here](https://github.com/LUMC-BioSemantics/phenopackets-rdf-schema/tree/v2/shex) and has also been adapted to SHACL whose files are provided [here](https://github.com/rosazwart/phenopackets-v2-rdf-schema/tree/main/shacl). The SHACL2YARRRML2RDF workflow can be found in [this repository](https://github.com/rosazwart/phenopackets-v2-rdf-schema).

## Future changes in phenopacket RDF 2.0

In case any changes are added to phenopacket RDF schema 2.0, the data in this folder needs to be replaced by the newly generated RDF data file. This new data file is acquired by rerunning the SHACL2YARRRML2RDF workflow on the SHACL files that are updated given the changes in the phenopacket RDF schema.

# References

[1]  Arindrarto, W., Borràs, D.M., de Groen, R.A.L. et al. Comprehensive diagnostics of acute myeloid leukemia by whole transcriptome RNA sequencing. Leukemia 35, 47–61 (2021). https://doi.org/10.1038/s41375-020-0762-8