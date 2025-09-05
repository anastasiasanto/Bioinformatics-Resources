# Bioinformatics-Resources
The aim of this project is to perform several analysis on cancer data, specifically on Lung Adenocarcinoma data, retrieved from 100 patients, including case and control groups. Bioinformatics Resources course a.a. 2023-2024
ANALYSIS : 
1. Load the RData file
2. Update raw_count_df and r_anno_df extracting only protein coding genes.  
3. Perform differential expression analysis using edgeR package and select up- and 
down-regulated genes using a p-value cutoff of 0.01, a log fold change ratio >1.5 for 
up-regulated genes and < (-1.5) for down-regulated genes and a log CPM >1.
4. Perform gene set enrichment analysis using clusterProfiler R package. 
a Perform both GO (BP and MF) and WP analysis  
b Report the top 10 enriched GO terms and the top 10 enriched WP pathways 
resulting from both up- and down-regulated gene lists 
5. Use the pathview R package to visualize one pathway you find enriched using the 
upregulated gene list.  
6. Identify which transcription factors (TFs) have enriched scores in the promoters of all 
up-regulated (or down-regulated if you prefer) genes.  
a use a window of 500 nucleotides upstream each gene  
7. Select one among the top enriched TFs, compute the empirical distributions of scores 
for all PWMs that you find in MotifDB for the selected TF and determine for all of 
them the distribution (log2) threshold cutoff at 99.75%. 
8. Identify which up-regulated (or down-regulated depending on the choice you made 
at point 7) genes have a region in their promoter (defined as previously) with binding 
scores above the computed thresholds for any of the previously selected PWMs.  
a Use pattern matching ì
9. Use STRING database to find PPI interactions among differentially expressed genes 
and export the network in TSV format.  
10.  Import the network in R and using igraph package and identify and plot the largest 
connected component.  
