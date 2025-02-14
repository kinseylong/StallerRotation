Kinsey's Rotation Spring 2025


cofactor_complexes: 
- data: manually curated csv files of cofactor subunits and paralogs
- cofactor_expression: datasets of tissue specifity of cofactor paralogs
- cofactors_old: analysis with non-normalized scRNA data
- cofactorcomplexes_mining.ipynb: 
    - API calling for ENSG ID to Gtex gene code
    - API calling for Gtex gene code to tissue expression profile from Gtex portal
- cofactor_analysis.ipynb: 
    - Clustering heatmaps of gene expression by tissue
    - Expression correlation between own-complex paralogs
    - KMeans and Agglomerative Clustering of subunits and tissue types
    - BAF-specific exploration in brain tissues
- cofactor_analysis_normalized.ipynb:
    - Same as above, but with normalized gene expression values across gene

cofactors_humanproteinatlas:
- data:
    - TF-AD-RD: directory containing .csv and .tsv files with ADs, RDs, and transcription factors from Lambert et al and Human Protein Atlas annotation.
    - proteinatlas-TFs.tsv: all proteins annotated as transcription factors in the Human Protein Atlas
    - proteinatlas-cluster34.tsv: all proteins in cell-specific expression cluster 34 (same as MED12L)
    - cofactors_mapped.tsv: Uniprot mapping tool results for manually curated cofactor subunits
    - cofactors_mapped_combined.tsv: Uniprot mapping and paralog/cofactor complex annotation for each subunit. cofactors_mapped.tsv merged with cofactor_complexes>data>cofactor_complexes_manual.xlsx
    - tfsmapped_gencodes.csv: Uniprot mapping for TFs from TF-AD-RD>tfs_combined.csv

- humanproteinatlas_mining.ipynb: 
    - API call to get scRNA-seq and Tau specificity scores from Human Protein Atlas
    - API call to get annotations from Human Protein Atlas
    - Application of API calls for cofactor subunits, ADs, RDs, transcription factors
    - Resulting .csv files are put in helperdata

- humanproteinatlas_analysis.ipynb:
    - Looking at cell-specificity and co-expression of paralogous cofactor subunits
    - Analysis of transcription factor co-expression




