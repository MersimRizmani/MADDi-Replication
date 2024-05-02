# Multimodal Attention for Alzheimer's Disease Classification

## Citation of Original Paper

Below are the references to the original research paper published to JAMIA, and the code repository:

Michal Golovanevsky, Carsten Eickhoff, Ritambhara Singh, Multimodal attention-based deep learning for Alzheimer’s disease diagnosis, Journal of the American Medical Informatics Association, Volume 29, Issue 12, December 2022, Pages 2014–2022, https://doi.org/10.1093/jamia/ocac168

GitHub Repository: https://github.com/rsinghlab/MADDi/tree/main

## General Problem

The general problem that this project focuses on is accurately diagnosing Alzheimer’s disease in susceptible patients. The objective of the original study was to develop a multimodal deep learning framework that could aid medical professionals in accomplishing this task and making Alzheimer’s diagnosis easier and more accurate. 

Why is it important to improve the process of Alzheimer’s disease diagnosis utilizing deep learning models? Well, according to statistics from Alzheimer’s News Today, Alzheimer’s disease is the most common neurodegenerative disorder affecting approximately 5.5 million people in the United States, and around 44 million people worldwide. On top of that, research has also shown that less than half of Alzheimer’s patients are diagnosed accurately for pathology and disease progression based on clinical symptoms alone. This statistic alone highlights the urgent need for advancement in Alzheimer’s disease diagnosis, and that is why deep learning researchers are working to create frameworks to solve this problem. 

## Approach

The approach taken by this research paper was centered around a multimodal deep learning framework called MADDi, short for Multimodal Alzheimer’s Disease Diagnosis framework. It utilizes a cross-modal attention scheme to integrate imaging data (i.e. MRI data), genetic data (i.e. SNPs), and structured clinical data to classify patients and attempt to label (diagnose) them. The entire pipeline involves clinical, image, and genetic data preprocessing, building the multimodal framework, neural network attention, unified hyperparameter tuning, and model evaluation.

In our project, we seek to replicate this study to the best of our ability by attempting to rebuild MADDi in our own notebook. From this process, our goal will be to fully understand and learn how real medical data, such as that from ADNI, can be paired with a functioning deep learning framework to greatly improve the accuracy of Alzheimer’s disease diagnosis.

## Hypothesis

The hypothesis we want to test according to this research paper is whether a novel multimodal deep learning framework, in this case MADDi, can accurately aid medical professionals in diagnosing Alzheimer’s disease. Specifically, we hypothesize that integrating multiple modalities (i.e. imaging, genetic, and clinical data) using a cross-modal attention scheme will lead to improved accuracy in Alzheimer’s diagnosis, compared to unimodal approaches. 

## Ablations

This project will involve the replication of two ablations, or experimental variations, presented in the original research paper:
Attention Mechanisms: Ablations will be conducted by toggling the presence of attention based on four criteria: self-attention and cross-modal attention, just cross-modal attention, and no attention. The variations will be generalized attention, self-attention, and cross-modal attention.
Unified Hyperparameter Tuning Scheme: Ablations will vary by toggling the methods for optimizing hyperparameters in the model. The scheme will allow for generalizing the model and tuning it for specific scenarios without manual intervention.

## Data Access

The data that will be processed and analyzed in this project and study replication has to be requested directly from the Alzheimer’s Disease Neuroimaging Initiative (ADNI). All ADNI data are shared without embargo through the LONI Image and Data Archive (IDA), a secure research data repository. Access is contingent on adherence to the ADNI Data Use Agreement and the publications’ policies.

Once access is granted from the LONI Image and Data Archive, which from our experience has a timeline of approximately two weeks, then we look for the necessary files in the data archive to download. In our case, we’d be looking for clinical, genetic, and imaging data from three studies: ADNI1, ADNI2, and ADNI GO.

## Computation Feasibility

In terms of computational feasibility, we believe we have all the resources required to reproduce this study. In terms of dependencies, the code seems to have dependencies on various python packages that should be easy to download. For computational power, if the code cannot be run locally, we could leverage more powerful resources using a platform like google colab. 

In terms of data for computation, we have obtained access to the clinical dataset the authors of the paper said was necessary. An obstacle we could see is usage of data since there are multiple datasets, so we will have to perform some exploration of the code and data to determine the correct datasets.

## Statement on the Use of Existing Code

For our project, we will be utilizing the existing code in an effort to replicate the original study. Specifically, we will attempt to replicate the MADDi framework that was developed in the original study. The original code can be found here: https://github.com/rsinghlab/MADDi/tree/main

## Using the code

To use our code, please look at the original repository (linked above), it is the same flow. To put it simply, to run the scripts use a command in the "python {script_name}". The jupytr workbooks can be run in google colab or like any other jupytr notebook.  

## Other References

Naqvi E. Alzheimer’s Disease Statistics. 2017. https://alzheimersnewstoday.com/alzheimers-disease-statistics/. Accessed June 20, 2022.

Thies W, Bleiler L. 2013 Alzheimer’s Disease Facts and Figures. Wiley Online Library; 2013. https://alz-journals.onlinelibrary.wiley.com/doi/10.1016/j.jalz.2013.02.003. Accessed June 20, 2022.
