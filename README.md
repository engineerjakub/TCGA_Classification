# TCGA_Classification

Genomic Biology is often characterized as a big data problem. Each individual human genome consists of ~3 Billion base pairs of DNA. Many of the chemical processes that occur in cell replication are a result of complex dynamic interactions between bases. Furthermore, each tissue in the body have different gene expression values that dicate whether it is activated/deactivated. The interactions of these expression values may point to a method of diagnozing cancer via. machine learning methods. Abnormal expression values allow for classification of different cancer types.

In this project, an ML pipeline is trained on gene expression values in 5 tissues most common to be cancerous in men:
- Bladder
- Lung
- Liver
- Prostate
- Colorectal

The TCGA (The Cancer Genome Atlas Program) Datasets were obtained from the UCSC Xena portal:
Xena Functional Genomics Explorer. (Accessed 2024) Xena functional genomics
explorer. [Online]. Available: https://xenabrowser.net/datapages/

For each patient, 20531 genes are sampled resulting in an enourmous dataset of 42.5 million total features. These are split 70/30 for training and testing.
The dataset was then reduced to 1.4 million features via. Principal Component Analysis (PCA) dimension reduction method.

Three models were trained on the data:
- Lasso Regression
- Decision Tree
- SVM

  The Lasso model performed the best with an F1 score of 0.99, indicating that the model was able to almost perfectly classify each of the 5 cancer types using only gene expression.


  
