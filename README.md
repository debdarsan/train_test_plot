# train_test_plot
A Python package to train, test, evaluate and plot confusion matrices, feature importance for classification problems

Performs the following operations:
---------------------------------
    
    1. Splits the dataframe into target (dependent variable) and predictors (independent variable)
    2. Scales the values of independent variables (all input values must be numeric)
    3. Splits the dataset into train and test sets
    4. Loops through the list of classification algorithms to
       a) Train
       b) Test
       c) Evaluate and report performance
       d) Plot Confusion Matrix
       e) Plot feature importance (if it is available for this particular algorithm)
    5. Shows comparative plot of accuracies for all the algorithms
       
    Parameters:
    ----------
       df (pandas dataframe): the whole dataset containing observations for both target and predictor variables
       target (string): column name of the target variable in df, e.g. 'Species'
       size (int): size of the plots, typical values are 5, 10, 15
       models: holding objects of classification models
       
    Returns:
    -------
        None
       
    Example:
    -------
       train_test_plot(iris_df, 'Species', 5, models)
       where,
            iris_df: input dataframe,  e.g. iris_df = pd.read_csv('Iris.csv')
            'Species': name of the target column in iris_df
            5: size of the plots generated
            models: list of model objects
            
## Installation

### pip install train_test_plot

## Files

#### 1. glass.csv (exapmle dataset)
#### 2. Example.ipynb (example usage notebook)
#### 3. Classifier.ipynb (complete source code)
