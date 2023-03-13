# Unsupervised Machine Learning

## Myopia Predictions using Unsupervised Machine Learning

I am on the data science team of a medical research company that’s interested in finding better ways to predict myopia, or nearsightedness. 
My team has tried—and failed—to improve their classification model when training on the whole dataset. 
However, they believe that there might be distinct groups of patients that would be better to analyze separately. 
So, my supervisor has asked you to explore this possibility by using unsupervised learning.

I have been provided with raw data, so I will first need to process it to fit the machine learning models. 
I will use several clustering algorithms to explore whether the patients can be placed into distinct groups. 
Then, I will create a visualization to share my findings with my team and other key stakeholders.

# Project Steps

## Part 1: Prepare the Data
1. Read myopia.csv into a Pandas DataFrame.
2. Remove the "MYOPIC" column from the dataset. ( The target column is needed for supervised machine learning, but it will make an unsupervised model biased ).
4. Standardize the dataset so that columns that contain larger values do not influence the outcome more than columns with smaller values.

## Part 2: Apply Dimensionality Reduction
1. Perform dimensionality reduction with PCA. How did the number of the features change?
2. Further reduce the dataset dimensions with t-SNE and visually inspect the results. To do this, run t-SNE on the principal components, which is the output of the PCA transformation.
3. Create a scatter plot of the t-SNE output. Are there distinct clusters?

## Part 3: Perform a Cluster Analysis with K-means
1. Create an elbow plot to identify the best number of clusters. Make sure to do the following:
2. Use a for loop to determine the inertia for each k between 1 through 10.
3. If possible, determine where the elbow of the plot is, and at which value of k it appears.

## Part 4: Make a Recommendation
* Based on your findings, write up a brief (one or two sentences) recommendation for your supervisor in your Jupyter Notebook. 
* Can the patients be clustered? If so, into how many clusters?

# Conclusion
* Can the patients be clustered?
1. Based on the amount of data that was made available, it's difficult to classify the patients.
2. There is not distinct cluster shown when using the t-SNE model.
3. The elbow curve chart was also not very distinct. It is more rounded than sharp elbow shaped.
4. This would not provide accurate information to the supervisor of this notebook.
