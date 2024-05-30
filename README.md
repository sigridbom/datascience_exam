# datascience_exam
The analysis was done in Visual Studio Code using Python version 3.12.3 on the UCloud interactive HP system, managed by the eScience at centre at SDU.


### Structure of notebooks
Notebooks are numbered (1,2,3) and they are supposed to be run in that order.
- 1_data_wrangling: Cleans, preprocesses and plots the data
- 2_embeddings: Embeds three different text columns and reduces their dimensions with PCA. PCA reduced embeddings are clustered for some of the embeddings.
- 3_building_models: Builds and tests different models. From a dummy 'mean' model to a RandomForestRegressor. 

### Data
The dataset is from Kaggle: https://www.kaggle.com/datasets/imoore/age-dataset (Annamoradnejad & Annamoradnejad (2022)

The data is uploaded in the data folder as a zipped file. 

The text embeddings used in the models are too big for GitHub even when zipped, so if you don't want to run the entire code, the files can be downloaded from here: https://drive.google.com/drive/folders/1ryos5F4kH5VcHczO7J7RyK33-x1YRduU?usp=sharing 
Those, which are nedded to run script 3_building_models, are called: test_features, val_features and train_features. 

### Models
Some models can be found in the /output/models/ folder, and others can be found in the linked google drive folder (due to size limits of GitHub).
Models on google drive include: KNN-regression, default random forest regression with all features and with a subset of features (58 predictors). 
Models on github include: the model object after the randomized cross-validation search and the tuned model which comes from that (technically, only the randomized search object is needed). 

### References
Annamoradnejad, Issa; Annamoradnejad, Rahimberdi (2022), “Age dataset: A structured general-purpose dataset on life, work, and death of 1.22 million distinguished people”, In Workshop Proceedings of the 16th International AAAI Conference on Web and Social Media (ICWSM), doi: 10.36190/2022.82

