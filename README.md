# TwoMonthLymphocyte
This repository analyzes data from collected from two subjects over two time points. 
This repository also compares the data to data from two CLL proteomics papers.

##Making Figure 1
Our experimental data was loaded using the longitudinal CLL package. Data was filtered 
to include relevant cell types and proteins seen in at least half the replicates. 
The data was normalized by log 2 transformation. T tests were run on the data and 
upregualted proteins were identified. The seaborn library allowed for creation of a 
volcano plot. Data was plotted on a volcano plot with upregulated proteins in orange.

##Making Figure 2
Relevant supplementary tables from Mayer et al. and Johnston et al. were downloaded. 
Data was parsed and sorted into differential and total proteins based on the qualifications 
from each paper. The matplotlib_venn library allowed creation of a venn diagram. Venn 
diagrams were created using total proteomic data and differential proteomic data from the 
two papers. The seaborn library was used to create a scatterplot. P-values for differential 
proteins in each paper were plotted on a scatterplot.  

##Making Figure 3
Relevant supplementary tables from Mayer et al. and Johnston et al. were downloaded. 
Data was parsed and sorted into differential and total proteins based on the qualifications 
from each paper. Our experimental data was loaded using the longitudinal CLL package. 
The matplotlib_venn library allowed creation of a venn diagram. A venn diagrams was 
created using total proteomic data from the two papers and our total proteomic data. 
We calculated the ratio of the differential proteins we identified to the total differnetial 
proteins of the two studies.

##Making Supplemental Table 3
Relevant supplementary tables from Mayer et al. and Johnston et al. were downloaded. 
Data was parsed and sorted into upregulated and downregulated proteins based on the 
qualifications from each paper. Using GProfiler we determined the KEGG pathways for each 
paper's upregulated and downregulated proteins.