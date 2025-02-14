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
        - TFs.csv: list of EnsemblIDs for transcription factors, used in mapping

    - humanproteinatlas_mining.ipynb: 
        - API call to get scRNA-seq and Tau specificity scores from Human Protein Atlas
        - API call to get annotations from Human Protein Atlas
        - Application of API calls for cofactor subunits, ADs, RDs, transcription factors
        - Resulting .csv files are put in helperdata

    - humanproteinatlas_analysis.ipynb:
        - Looking at cell-specificity and co-expression of paralogous cofactor subunits
        - Analysis of transcription factor co-expression

    - mediator_exploration.ipynb
        - Cell-specificity of mediator subunits
        - Identifying co-expressed transcription factors
        - Annotations of co-expressed transcription factors
        - Identifying co-expressed AD/RDs
        - Exploring Cluster 34 (MED12L similar) proteins

    - BAFexploration.ipynb
        - Cell-specificity of BAF subunits

    - BAF_exploration2.ipynb
        - Cell-specificity of BAF subunits in more detail
        - Measuring co-expression between own-complex BAF paralogs vs all BAF pairs 

    - TFspecificity-old.ipynb
        - Cell-specificity and co-expression of full TF list, and AD/RDs
        - Sequence motifs, compositional bias, etc. (from Uniprot annotations) of co-expressed TFs 

mediator
    - data: sequences of Mediator subunits, Foldseek results, ALBATROSS results, metapredict results
    - phylo_raw: Phylo scores of MED12/12L by base pair from UCSC genome browser 
    - ..._exon_positions.csv: exon coordinates for MED12 and 12L genes
    - MED12_12L_structure.ipynb:
        - Map disordered regions of MED12 and MED12L
        - Sequence comparison and alignment of disordered regions
        - Sequence feature comparison of disordered regions
        - Manually-selected motif counting and comparison 
        - ALBATROSS comparison for tail IDR


finches
    - virtual environment to fun FINCHES

