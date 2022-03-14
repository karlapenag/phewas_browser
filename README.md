## PheWAS browser

### Dependencies
install.packages(c("shiny", "rio", "here", "plotly",'DT', 'flexdashboard', 'ggplot2', 'leaflet'))

devtools::install_github("karlapenag/phewas_browser")

### Run dashboard

rmarkdown::run("index.Rmd")

### Data Collection and Filtration

The whole data (215,107) was downloaded from PheWAS catalog. The data was filtered following these criteria:
- Variants with gene name (remove NULL & weird excel formatting with dates)
- No chromosome X because caused some issues in R (cells automatically erased because identified column as numerical)
- Randomly deleted 214,106 rows. Kept 1,001 for easier work in R.

Modifications:
- Separated first column (chromosome) in two (chr & pos) by comma.
- Added logPvalue
- Sorted by chromosome (ascending)
- Saved as .xlsx (not .csv)

Created but not used:
- Excel file with only the unique separated-by-comma gwas-associations of the filtered file in one column for future use.


## Download data from phewas-catalog
 
 Link to PheWAS website
 https://phewascatalog.org/phewas
 
 Link to download dataset
 https://phewascatalog.org/files/phewas-catalog.csv.zip