**Title of Project**: **"Autoencoder Imputation of Missing Heterogeneous Data for Alzheimer’s Disease Classification."**                The current repository consists of a deep neural network approach of imputing the missingness in the heterogenous ADNI data.        Google Colab (https://colab.google/), a cloud-based Jupyter notebook environment provided by Google, was utilised for conducting the study, which included data preprocessing, feature selection, missing data generation (40% - 70%, imputation using denoising autoencoder, classification using Random Forest Classifier and validations.

**Dataset**:
The dataset used in the study was obtained from ADNIMERGE-3 open repository as per request.

**Repository Files**:

Following order of the files demonstrating the project;

Data_Preprocessing_steps.ipynb : Code for data preparation and preprocessing steps including normalisation.
Feature_selections.ipynb : Code for extracting important features using Boruta, logistic regression with L1 regularization and autoencoder.
Original_dataset_Classification.ipynb : Code for the random forest classification (3 class classification) of the original dataset followed by SMOTE.
Dataset_with_MOTHDEM_column_missing_imputation&Classification.ipynb : Code for generating missingness of 40%, 50%, 60% and 70% in the MOTHDEM column followed by imputation using DAE and classification using Random Forest Classifier.
Dataset_with_missingness_in_APoE_column_imputation&Classification.ipynb : Code for generating missingness of 40%, 50%, 60% and 70% in the APoE column followed by imputation using DAE and classification using Random Forest Classifier.
Dataset_with_missingness_in_CDR_column_Imputation&Classification.ipynb :  Code for generating missingness of 40%, 50%, 60% and 70% in the CDR column followed by imputation using DAE and classification using Random Forest Classifier.
Classification_of_Feature_selected_dataset.ipynb : Code for the classification of the selected features obtained from the employed traditional feature selection methods and from the denoising autoencoders on each imputation. 

**Usage of the project**:
1. Data Preprocessing: Open the python Jupyter Notebook and run the codes for data preparation and preprocessing. This includes removal of irrelevant column, standardisation of the gender column, transformation of negative values to non - negative values and normalisation of the features.
2. Feature Selection: Employ the feature selection methods;Boruta,logistic regression with L1 regularization and autoencoder.
3. Generation of missingness, Imputation and Classification: Select the features that highly relate to Alzheimer's disease severity and generate different levels of missingness, then impute the missingness using the code for DAE and classify using Random Forest Classifier.
4. Evaluation: Evaluate the performance of the model by running the code for calculating accuracy, precison, recall and F1 score.

**License**
The current project is licensed by 'GNU General Public License v2.0'.


