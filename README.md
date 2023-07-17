# 2022-topic-05-team-04: breast cancer

**Team:** Simon Westermann, Sharujan Suthakaran, Aaron Eidenmüller, Luis Herfurth
<br/> **Supervisor:** Prof. Dr. Carl Herrmann
<br/> **Tutor:** Ana Luisa S. Costa

# Drug viability screens for oncological and non-oncological treatments

## Abstract 
Breast cancer still presents a significant global health challenge, requiring improved treatment options with minimized side effects. Since traditional drug development is costly, time-consuming, and risky, progress is hindered. Drug repurposing offers a potential solution by finding new applications for approved drugs, therefore reducing costs and development time.\\
This research project focuses on a computational approach, utilizing genetic associations to identify target genes for drug development. By analysing treatment response and genetic data, including gene expression profiles, the research project aims to identify promising gene candidates as potential drug targets. These genes were evaluated  by assessing gene knockout scores and drug effectiveness of associated treatments at different treatment doses could be predicted. The goal is to contribute to personalized and efficient treatment options for breast cancer patients.\\
It was shown that associations between genes and treatments could be made even though with only slight potential for drug repurposing use. However, predicting treatment response by drug dose is able to accurately help in evaluating potential drug repurposing candidates. In general, this research project highlights an approach in finding new gene targets and drugs applications by analysing genetic data and evaluating the potential usefulness of such repurposed drugs.

## Our data
Seven datasets were provided for further data analysis. These datasets can be divided into to two subsets, the PRISM datasets and gene-related datasets.
Our main PRISM dataset describes treatment response on cell growth of different cell lines. Assigned columns are code ID names from the treatments and the cell lines are ordered row-wise. The values represent the log 2 fold change in comparison with a DMSO experiment and are referred to as prism scores. Additional information about the treatments used in PRISM can be found in the second dataset including its mechanism of action, common purpose and more. Lastly, the PRISM cell line data set presents detailed information about all cell lines and their cancer origin.
Furthermore, the three of the four given gene-related datasets present gene designations as column names and cell line IDs as row names, each containing different measurement values.
The expression data frame describes expression levels of each gene in different cell lines. The copy number data frame contains the copy number of each gene for every cell line used in the PRISM screen. The gene importance data frame displays the gene importance measured by knockout scores of each gene in every cell line. With different format the last gene-related data set offers valuable information about the gene including the common function, mutation and more.
 
## Our Repository

**01_DataCleaning/Filtering:** Cleaning of the different datasets and filtering of the data to prepare for downstream analysis.

**02_DescriptiveAnalysis:** Gene search engine and descriptive analysis of the data.

**03_DimensionReduction:** UMAP and PCA of filtered data

**04_GeneAnalysis:** Correlation between gene expression and gene copy number and statistical testing of important genes

**05_LinearRegression:** Linear regression between concentration and average prism score for every drug

