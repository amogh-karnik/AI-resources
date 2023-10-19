**Assignment: The project proposals should be a single PDF file less than two pages in length and  cover the following four points:**  
### What task will you address, and why is it interesting? 
*(This can be as simple as a couple of sentences.)*

We are going to be examining the biology of aging in a population of Amish individuals. We will be using data aggregated from previous studies which examined in particular, a loss-of-function mutation in the gene encoding PAI-1 (*plasminogen activator inhibitor-1*), and its relationship with enhanced longevity in this specific population. We have a number of features including clinical phenotype data (vital signs, blood work, and imaging results), RNA transcriptome data, proteomics data, and DNA-methylation data.  Patients have also been classified by their genotype at the PAI-1 locus.

See the published research article at: https://www.science.org/doi/10.1126/sciadv.aao1617
### How will you acquire your data?

The three project members are already included on an IRB-approved research team with approval to directly access all of the data. There are a number of data sets which will require cleaning and de-identification, prior to merger for inclusion in the overall analysis.
### Which features/attributes will you use for your task?  

We will be working primarily with the clinical phenotype for the first task, a classification task developing a model to classify PAI-1 genotype status (wild-type, heterozygote, homozygote) using only these clinical data. 

For the second task, we will incorporate other -omics data as available.

### What will your initial approach be? 
#### What data pre-processing will you do?

We will need to de-identify the data by removing any potential personally-identifiable information. Exploratory Data Analysis will be performed to examine the attributes and assess any correlation between features. Features with a high degree of missingness will be excluded. Missing values will be imputed based on mean for normally distributed variables or median for skewed distributions. The mode will be used for categorical variables. Continuous data will require normalization.

#### Which machine learning techniques (decision trees, KNN, K-Means, Gaussian mixture models, etc.)   will you use?

We plan to use a KNN model for the classification task looking at the PAI-1 genotype classification for patients based on phenotypic information.

We will use a Gaussian Mixture Model for the regression based on chronological age. 

#### How will you evaluate your success (Note: you must use a quantitative metric)? 
*(Generally you will likely use mean-squared error for regression tasks and precision-recall for classification tasks. Think about how you will organize your model outputs to calculate these metrics.)*

