# Ranked_MSD

## A New Feature Ranking and Feature Selection Approach

#### Research Question: Can we identify a reasonably small subset of important genes for a particular disease by analysing gene expression profiles without losing disease prediction accuracy?

#### Algorithm 1. Ranked_MSD_F_Best: This algorithm can rank all the features based on their importance score and select a small subset of features that can give best accuracy without losing disease prediciton accuray.

#### Algorithm 2. Ranked_MSD_F_Equal: This algorithm can rank all the features based on their importance score and select a small subset of features that can give accuracy equal to the full feature set.

The uploaded codes demonstrate the algorithms performance using k-NN classifier. Proposed algorithms can be tested using any machine learning classifier. Just change KNN training code to any other classifier that you want to use.

### Abstract:

In the era of big data when a huge amount of data is continuously being generated, it is common for situations to arise where the number of samples is much smaller than the number of features (variables) per sample. This phenomenon is often found in biomedical domains, where we may have relatively few patients, compared to the amount of data per patient. For example, gene expression data typically has between 10,000 and 60,000 features per sample. A separate issue arises from the "right to explanation" found in the European General Data Protection Regulation (GDPR), which may prevent the use of black-box models in applications where explainability is required. In such situations, there is a need for robust algorithms which can identify the relevant features from experimental data by discarding irrelevant ones, yielding a simpler subset that facilitates explanation. In this work, we have aimed to tackle the issues that arise when the number of samples is much smaller than the number of features (commonly referred to as n ≪p). It becomes very hard to interpret the target concept in these situations. In addition, irrelevant features often confuse machine leaning systems and lead to deterioration of classification accuracy. Furthermore, machine learning with irrelevant features increases computation time and memory requirements. To address these problems, we have proposed a feature ranking algorithm named Ranked MSD with two additional algorithms to identify strongly relevant features (F_Equal feature set) and all the relevant features (F_Best feature set) by discarding irrelevant features. Our experimental results show that the proposed Ranked MSD algorithm outperforms two well-known feature ranking methods, Correlation Criteria and Information Gain. 

We have tested our proposed approach on two real-world gene expression data sets, both of which relate to respiratory viral infections. This Ranked MSD feature selection algorithm is able to reduce the feature set size from 12,023 genes (features) to 65 genes on the first data set and from 20,737 genes to 31 genes on the second data set, in both cases without any significant loss in disease prediction accuracy. In an alternative configuration, our proposed algorithm is able to identify a small subset of features that gives better accuracy than that of the full feature set. Our proposed algorithm can also identify important biomarkers (genes) with their importance score for a particular disease.

This work is published in CD-MAKE 2019 Conference. Link to the published paper: https://link.springer.com/chapter/10.1007/978-3-030-29726-8_10
