This repository contains files necessary to run a gene prioritization pipeline to identify 'clinically-relevant' genes that have been previously associated with risk for Autism Spectrum Disorders (ASD).

Files required to complete the pipeline are as follows:
1. 'disease_mappings.tsv'= all of the Unified Medical Language System (UMLS)® Concept Unique Identifiers (CUI) and genes associated with these terms available in DisGeNET

2. 'E-MTAB-5214-query-resultsbrain_TPM.tsv'= all genes that have been found expressed at a default cut-off level of TPM≥0.5 in human brain tissue from RNA-Seq conducted for the Genotype Tissue Expression (GTEx) project
Alternative 2. If the FPKM values are preferable, 'E-MTAB-5214-query-results.tsv'= all genes that have been found expressed at a default cut-off level of FPKM≥0.5 in human brain tissue from RNA-Seq conducted for the Genotype Tissue Expression (GTEx) project 

3. 'MouseKO_ASDtraitsgenes_hsortho.xls'= genes that when knocked out of mice have been observed to have a phenotypic consequence that relates to  'nervous system development' and/or a 'behavioral/neurological phenotype' as defined by the International Mouse Phenotyping Consortium

Output files useful for more detailed descriptions of annotations include:
1. 'ASDRiskGeneAttributes.csv'= final data frame with all gene attributes of interest to visualize

2. 'ASD_ACMGPPIs_details.csv'=details for the specific protein-protein interactions that were predicted between ASD risk proteins and American College of Medical Genetics proteins that are recommended to test for pathogenic variants

3. 'ASDRiskGeneMouseKOTraits_details.csv'=Details as to the specific ASD-related traits that were observed when the ASD risk gene was knocked out of a mouse model

4. 'ASDRiskGenes.in.SigGOBioProcess_details.csv'=For each ASD risk gene this file contains details regarding each biological process defined by Gene Ontology that was significantly over-represented for ASD risk genes to which the gene was assigned
