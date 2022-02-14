Telco Customer Churn Prediction
A comparison study of Logistic Regression and Random Forest
--------------------------------------------------oo----------------------------------------
INM-431 Machine Learning Coursework 
Elnara Mammadova - 210025788


=========================== HOW TO TEST =====================================
Please run matlab livescript "testing.mlx" to test the final model.
All the necessary data has been loaded. 
The codes were run in university computers without a glitch. 


======================= WHAT IS INCLUDED IN THE FOLDER ======================
All the preprocessing, modelling and testing steps are completely reproducible 
and all necessary data is contained in this folder. 

1. "Data_Preperation.ipynp" included:
    - data understanding - visual analysis 
    - outlier removal
    - feature engineering 
            - encoding discrete features 
            - standarization of continious features
    - data splitting - training and testing 
    - SMOTE method on training data 
    
    input: "Telco_customer_churn", "churn.csv"
    output: "churn_postprocess.csv", "train.csv", "train_balanced.csv", "test.csv"
    
    Jupyter Versions: 
    seaborn==0.11.0
    plotly==5.4.0
    pandas==1.1.3
    numpy==1.19.1
    matplotlib==3.3.1
    
    
2. "MLCourseworkFinal_EM.mlx"
    - Single matlab livescript containing training, tuning, testing of all models
    - in order to reproduce add "data" folder to the path
    
    input: "churn_postprocess.csv", "train.csv", "train_balanced.csv", "test.csv"
    output: "MLCourseworkFinal_EM.mat"(not included in the submission due to size),
	    "finalModels.mat" (included in the submission files)

3.  "GridSearch.mlx"
    - Single matlab livescript containing hyperparameter optimization for Random Fores
    - Total of 14 Grid Search results. "GStable14" containes the last and final results.
    
    input: "train.csv", "train_balanced.csv", "test.csv"
    output: "GridSearch.mat"  (not included in the final submission due to size)
    
4. "testing.mlx"
    - the file required for the grader to run. .mat file already loaded. Press RUN to see the results
    
    input: "finalModels.mat"
    output: none
    
    Matlab Version: 
-----------------------------------------------------------------------------------------------------
MATLAB Version: 9.10.0.1739362 (R2021a) Update 5
MATLAB License Number: 902060
Operating System: macOS  Version: 11.4 Build: 20F71 
Java Version: Java 1.8.0_202-b08 with Oracle Corporation Java HotSpot(TM) 64-Bit Server VM mixed mode
-----------------------------------------------------------------------------------------------------
MATLAB                                                Version 9.10        (R2021a)
Bioinformatics Toolbox                                Version 4.15.1      (R2021a)
Curve Fitting Toolbox                                 Version 3.5.13      (R2021a)
Deep Learning Toolbox                                 Version 14.2        (R2021a)
Reinforcement Learning Toolbox                        Version 2.0         (R2021a)
Statistics and Machine Learning Toolbox               Version 12.1        (R2021a)

All modelling codes were written in matlab. 