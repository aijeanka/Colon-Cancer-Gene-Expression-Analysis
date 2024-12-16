# **Colon Cancer Gene Expression Analysis**

## **Project Overview**

This repository contains data, code, and results for a gene expression study on colon cancer patients. The primary goal is to identify differentially expressed genes associated with relapse by comparing gene expression profiles between patients who relapsed and those who did not. The analysis leverages statistical testing, data visualization, and reproducible workflows implemented in R Markdown.

---

## **Highlights**

- **Packages Used**:  
  - `tidyverse` – Data manipulation and visualization  
  - `limma` – Linear models for microarray and RNA-seq data  
  - `knitr` – Dynamic report generation  
  - `DT` – Interactive data tables  
  - `ggplot2` – Data visualization  

- **Code**:  
  R Markdown script for performing and documenting the analysis.

- **Reproduced Figure**:  
  A visual summary of the top 20 differentially expressed genes and T-test results.

---

## **Repository Organization**

For improved reproducibility and clarity, the repository is organized into the following directories:

```
Colon_Cancer_Analysis/
│
├── data/              # Raw and processed data files
│   ├── Aizhan_Uteubayeva_ClinBaseIDs.tsv
│   ├── Aizhan_Uteubayeva_ClinCompIDs.tsv
│   ├── Aizhan_Uteubayeva_GeneExpBaseIDs.tsv
│   ├── Aizhan_Uteubayeva_GeneExpCompIDs.tsv
│   ├── Aizhan_Uteubayeva_FeatureIDs.tsv
│   ├── StudentName_Checking.xlsx
│   └── Aizha-Uteubayeva-TTestHW-05-Top20Genes.tsv
│
├── scripts/           # R Markdown scripts and compiled reports
│   ├── Aizhan-Uteubayeva-TTestHW-02-a-Code.Rmd
│   └── Aizhan-Uteubayeva-TTestHW-02-b-Code.html
│
├── results/           # Output files and analysis results
│   └── Aizhan-Uteubayeva-TTestHW-04-Output.csv
│
├── docs/              # Project documentation
│   └── Aizhan-TTestHW-01-Logic.pdf
│
└── LICENSE            # License information
```

### **Explanation of Directories**

1. **`data/`**: Contains all raw and processed datasets required for the analysis.
2. **`scripts/`**: Includes the R Markdown script (`.Rmd`) for running the analysis and the compiled HTML report (`.html`).
3. **`results/`**: Stores output files such as T-test results and lists of differentially expressed genes.
4. **`docs/`**: Project documentation and analysis logic plan.
5. **`LICENSE`**: Licensing information for the project.

---

## **Files and Descriptions**

### **Data Files**

- **Clinical Group IDs**:  
  - `Aizhan_Uteubayeva_ClinBaseIDs.tsv`: Baseline group patient IDs  
  - `Aizhan_Uteubayeva_ClinCompIDs.tsv`: Comparison group patient IDs  

- **Gene Expression Group IDs**:  
  - `Aizhan_Uteubayeva_GeneExpBaseIDs.tsv`: Baseline group gene expression IDs  
  - `Aizhan_Uteubayeva_GeneExpCompIDs.tsv`: Comparison group gene expression IDs  

- **Feature Data**:  
  - `Aizhan_Uteubayeva_FeatureIDs.tsv`: List of gene features used in the analysis  

- **Top Genes**:  
  - `Aizha-Uteubayeva-TTestHW-05-Top20Genes.tsv`: Top 20 differentially expressed genes  

- **ID Check**:  
  - `StudentName_Checking.xlsx`: Verification of patient IDs between clinical and gene expression datasets  

### **Scripts**

- **R Markdown**:  
  - `Aizhan-Uteubayeva-TTestHW-02-a-Code.Rmd`: Script to perform the differential gene expression analysis  

- **Compiled Report**:  
  - `Aizhan-Uteubayeva-TTestHW-02-b-Code.html`: HTML output from the R Markdown script  

### **Results**

- **T-Test Results**:  
  - `Aizhan-Uteubayeva-TTestHW-04-Output.csv`: Results of the T-tests, including p-values and fold changes  

### **Documentation**

- **Analysis Plan**:  
  - `Aizhan-TTestHW-01-Logic.pdf`: Overview of the analysis logic and methodology  

---

## **Steps to Reproduce the Analysis**

1. **Set Up Environment**:  
   Ensure the following R packages are installed:  
   ```r
   install.packages(c("tidyverse", "limma", "knitr", "DT", "ggplot2"))
   ```

2. **Clone the Repository**:  
   ```bash
   git clone https://github.com/yourusername/Colon_Cancer_Analysis.git
   cd Colon_Cancer_Analysis
   ```

3. **Prepare the Data**:  
   Ensure all data files are placed in the `data/` directory.

4. **Run the Analysis**:  
   Execute the R Markdown script:  
   ```r
   rmarkdown::render("scripts/Aizhan-Uteubayeva-TTestHW-02-a-Code.Rmd")
   ```

5. **View the Report**:  
   Open the compiled HTML report in the `scripts/` directory:  
   `scripts/Aizhan-Uteubayeva-TTestHW-02-b-Code.html`

6. **Review Results**:  
   Results and outputs can be found in the `results/` directory.

---

## **Key Analysis Steps**

1. **Data Import**: Load clinical and gene expression datasets.
2. **Data Cleaning**: Align and verify patient IDs.
3. **Group Comparison**: Perform T-tests to identify differentially expressed genes.
4. **Results Export**: Output significant genes and T-test statistics.
5. **Visualization**: Generate plots to illustrate the top findings.

---

## **Contributing**

Contributions are welcome! Please follow the guidelines in the `CONTRIBUTING.md` file.

---

## **License**

This project is licensed under the **MIT License**. See the `LICENSE` file for details.

---

## **Author**

**Aizhan Uteubayeva**  
*Initial analysis and documentation.*
