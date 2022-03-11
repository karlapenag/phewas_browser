### PheWAS browser

##

---

## Background


## Our approach

### Data Collection and Curation

Data was collected from PheWAS catalog (). This data was filtered (162,829)
sorted by chromosome number
deleted: bp, odds ratio, phewas code
fileterd: gene name: null & weird month done by excel

### Requirements
install.packages(c("shiny", "dplyr", "htmlwidgets", "digest", "bit"))
devtools::install_github("karlapenag/phewas_browser")

### Run dashboard
rmarkdown::run("phewas-browser.Rmd")

**Our role in the project is described in the following paragraph:**

The possibility of identifying statistically significant associations based on rare variants decreases with decreasing frequency of the allele. Consequently, **rare and unique variants need to be grouped together** in the most meaningful way. Most commonly, variants are grouped at the gene level. However, most eukaryotic proteins have more than just one functional site, and mutations can have mild to severe effects on each function, depending on their position within the 3-dimensional (3D) protein structures. Consequently, grouping on a gene level leads to mixing of variants that cause different and even opposing phenotypes. Such incoherent binning may mask menaningful associations. Here we will improve on the current state-of-the-art of gene binning in two ways. Firstly, we will use our expertise in the structural analysis of genetic diseases to develop a **3D structure-based filtering method**.


(The following will be done by Jesper Tegner's lab) Secondly, the set of genetic variants will be analysed in reference to their tissue and cell specificity. We will use the integration of protein-protein interaction data and their respective tissue and cell specificity, as supported by single cell transcriptomics data. This provides a biological context for grouping of variants as well as functional prediction.

### 3. Statistical analysis

We will then integrate the information of the variants within each bin to enhance the signal for association. We will apply the burden test, which calculates a burden score for a group of variants. We will try different options of the burden test [...] We will then conduct **phenome-wide association study (PheWAS)** between the integrated risk scores, and the clinical diagnoses and quantitative clinical lab measures from KFSHRC. In order to showcase the power of the local population, we will compare the results from our local **2,000 patients** with the data generated using an equivalent sample size taken at random from the **UK BioBank dataset** [...]

## Expected impact



## Download data from phewas-catalog


