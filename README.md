# tcga_brca1_data_analysis
 excessive data analysis for BRCA1 mutation in TCGA study 

clinical data and the mutation sub-category is retrieved from -
https://portal.gdc.cancer.gov/repository?facetTab=cases&filters=%7B%22op%22%3A%22and%22%2C%22content%22%3A%5B%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22cases.project.project_id%22%2C%22value%22%3A%5B%22TCGA-BRCA%22%5D%7D%7D%2C%7B%22op%22%3A%22in%22%2C%22content%22%3A%7B%22field%22%3A%22files.data_category%22%2C%22value%22%3A%5B%22Clinical%22%5D%7D%7D%5D%7D&searchTableTab=cases

this project retrieves clinical data and a subcategory for patients with BRCA1 mutation (code can be altered to a different mutation or for any other subgroup). after receiving the data, the script preforms a few exploratory analysis with plots.

the second part of the analysis preforms, based on the TCGA_BRCA gene expression table, an anova test with a Tukey-HSD post-hoc test for each gene, per the 4 groups that were decided (Mutation/wild_type - early on set/late on set). Results will be shown for the significant genes based on selected p-value. Combination for three test could be preformed for different age criteria, resulting for each gene, if it was significant in one, two or for all the tests.

TCGA_BRCA.csv - gene expression table must be downloaded outside of the Github repository because of its size over 100mb