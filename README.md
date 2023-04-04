# networks_motifs

Summary of Workflow for Integrative approach:

1.Based on the binding profiles for STAT1, STAT2, IRF1 and IRF9, TF-specific gene lists were prepared (e.g. STAT1-target genes).

2.The motif file containing GAS-only, ISRE-only and composite containing genes were generated (by others).

3.The integration analysis was performed using genes from RNA-seq and the merged peaks from CHIP-seq. Briefly, BETA tool was run using this script(nested_all_beta.sh), followed by extraction of upregulated genes from all time points and combining all files into a single one (cat file1.txt file2.txt file3.txt | sort > file4.txt). Then, the integrative gene list was initially refined by the identification of overlapping genes between the integrative list and the gene lists from step 1, followed by the detection of integrative genes that share a motif site based on the list from step 2. Accordingly, the number of refined integrative genes were 330 and 308, in IFNa- and IFNy-treated groups, respectively. Please check "clusters.ipynb" script (Refined gene list) for the latest integrative gene list.


