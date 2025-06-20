# GBM_IntrinsicDrugResistance

Files available: 

- Compiled RNA-seq count matrix (.xlsx)
  - Contains raw read counts, representing the number of sequencing reads mapped to a particular gene
  - Rows as genes and columns as samples
    
- Compiled global CpG island methylation matrix (.xlsx)
  - Contains raw methylation values (%), calculated as the fraction of methylated reads over total reads (beta value) at a specific CpG island
  - Rows as CpG islands and columns as samples
    
- Raw global CpG island methylation data for each individual sample (.bed files)
  - Contains raw methylation values (%) of each CpG site within CpG islands for each sample
  - Bed file column format, as assessed by Nanopore Technologies Modkit
  - Relevant columns: 
    - 1 - Chromosome number
    - 2 - Start position of the CpG site
    - 3 - End position of the CpG site
    - 4 - Modified base code (5mC)
    - 5 - Valid coverage
    - 8 - Color (always 255,0,0)
    - 10 - Methylation level as percentage at the CpG site
    - 11 - Number of calls passing filters classified as methylated
    - 12 - Number of calls passing filters classified as the canonical base rather than modified
    - 13 - Number of calls passing filters classified as other modification
    - 18 - Chromosomal location of the CpG island
    - 19 - Start position of the CpG island
    - 20 - End position of the CpG island
    - 21 - Unique CpG island ID
      
- DNA coordinates for each CpG island used in the study (.txt)
  - Contains specific genomic locations (chromosome, start, end) of each CpG island analyzed in the study 
