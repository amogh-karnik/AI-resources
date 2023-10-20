**Assignment: The project proposals should be a single PDF file less than two pages in length and cover the following four points:**

1. What task will you address, and why is it interesting?

We will examine the biology of aging in a population of Amish individuals. We will be using data aggregated from previous studies which examined in particular, a loss-of-function mutation in the gene encoding PAI-1 (*plasminogen activator inhibitor-1*), and its relationship with enhanced longevity in this specific population. We have a number of features including clinical phenotype data (vital signs, blood work, and imaging results), RNA transcriptome data, proteomics data, and DNA-methylation data. Patients have also been classified by their genotype at the PAI-1 locus.

[This article by Khan et al](https://www.science.org/doi/10.1126/sciadv.aao1617) will be used as a reference point for our work. 


2. How will you acquire your data?

The three project members are already included on an FSM IRB-approved research team with approval to directly access all of the data. There are a number of data sets which will require cleaning and de-identification, prior to merger for inclusion in the overall analysis.

3.  Which features/attributes will you use for your task?

We will be working primarily with the clinical phenotype for the first task, a classification task developing a model to classify PAI-1 genotype status (wild-type, heterozygote, homozygote) using only these clinical data. We will use basic demographic information, vital signs (blood pressure, heart rate, oxygen saturation), blood tests (blood counts, serum chemistries, cardiac biomarkers), echocardiogram results, cardiopulmonary exercise testing results, pulmonary function testing results, among other clinical data attributes. We do not intend on exploring the use of genomics, proteomics, DNA methylation data, and RNA sequence data at this stage, but will consider exploring how these attributes affect our model's performance pending additional exploratory data analysis. 

3.  What will your initial approach be?
	- What data pre-processing will you do?
		We will need to de-identify the data by removing any potential personally-identifiable information. Exploratory Data Analysis will be performed to examine the attributes and assess any correlation between features. Features with a high degree of missingness will be excluded. Missing values will be imputed based on mean for normally distributed variables or median for skewed distributions. The mode will be used for categorical variables. Continuous data will require normalization.

  
	- Which machine learning techniques (decision trees, KNN, K-Means, Gaussian mixture models, etc.) will you use?
		We plan to use a K-nearest neighbors model for the classification task looking at the PAI-1 genotype classification for patients based on clinical information. 
		
	- How will you evaluate your success (Note: you must use a quantitative metric)?
		We intend on using a precision-recall framework in order to evaluate the effectiveness of our classification model. Given that we are looking for a model to balance both precision and recall, we will calculate an F1 score to assess the overall model performance. 