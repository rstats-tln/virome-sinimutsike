# Human gut virome composition and dynamics in T2D patients receiving Metformin 

## Data

**data/phage_counts.csv** contains gut metagenomic shotgun reads that were assigned to division phages from study of newly diagnosed T2D patients receiving either metformin or placebo (study accession: PRJNA361402). Samples were collected at three timepoints: before treatments, 2 months after start of treatment and 4 months after start of treatment. All patients were also on calorie restriction diet during the study.

Viral sequences identification and taxonomic assignment was done using virome_quant bioinformatic workflow (https://github.com/avilab/vs).

phage_counts data is a 2% sample from full dataset and contains 6 variables: 

- *subject*: patient id.
- *arm*: treatment arms P (placebo) and M (metformin).
- *timepoint*: study timepoints, 0 is a pre-treatment baseline, 2 and 4 are months after the start of treatment.
- *query*: unique sequencing read id.
- *tax_id*: taxon id assigned to query.
- *parent_tax_id*: parent taxon id assigned to query.

Data can be summarised either at the level of taxon_id or parent_taxon_id. 

**data/library_size.csv** number of total sequencing reads in metagenomic shotgun library (can be used for normalisation). Note that phage_counts is a 2% sample.

1)import data
2)summarize
3)visualize
