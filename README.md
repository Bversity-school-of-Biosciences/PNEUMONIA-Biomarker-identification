# PNEUMONIA-Biomarker-identification
Hey there, this project involves the analysis of gene expression data to identify potential biomarkers for pneumonia. 
The workflow includes data collection from GEO (Gene Expression Omnibus), data filtering and processing, functional annotation using **DAVID**
and visualization of the identified biomarkers with **Tableau**.

# Biomarker Identification for Pneumonia Using Gene Expression

Installation
To replicate this project, ensure that you have the following tools and software installed:
- [DAVID Bioinformatics Resources](https://david.ncifcrf.gov/)
- [Tableau Desktop](https://www.tableau.com/)

Data Collection
The gene expression data used in this project was obtained from the **GEO database**. The specific dataset utilized can be found [here](https://www.ncbi.nlm.nih.gov/geo/).

Data Preparation
1. Download the dataset in **.txt** or **.csv** format.
2. Analyse the significant values using TWO TAILED T-TEST.
3. FORMULA= T.Test(Array 1, Array 2,tails,type)
              Array1 = healthy sample
              Array2 = Diseased sample
              Tails  = difference in both direction (Higher/Lower)
              Type   = Paired data, Two sample equal variance, Two sample with unequal variance.
5. Filter and process the data to retain only significant genes  (P value: <0.005 and fold change: >2)

Workflow
### 1. Functional Annotation with DAVID
- Upload the filtered gene list to **DAVID**.
- Select the appropriate gene identifier type (e.g., **ENSEMBL Gene ID**, **official_Gene_symbol**).
- Perform functional annotation to identify significant pathways and biological processes.

### 2. Data Visualization with Tableau
- Export the DAVID results.
- Import the data into **Tableau Desktop**.
- Create visualizations such as bar charts, scatter plots, or heatmaps to represent key findings.

Results
The visualizations produced in Tableau provide insights into the most relevant biological pathways and gene clusters associated with pneumonia, helping to identify potential biomarkers.
## Project Structure
