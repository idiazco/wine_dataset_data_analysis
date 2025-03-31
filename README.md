# wine_dataset_data_analysis
 A little data analysis of the wine dataset from sklearn.

## **DATA**

The dataset used for this practice is the one from sklrean [Wine](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_wine.html). It is classic dataset and very useful for multi-class classification. 

## REDUCTION OF DIMENSIONALTY PCA VS TSNE
In this practice, we investigate a little bit about how to recude dimensionaly, which method is better, and what outcome we obtain.

### PRINCIPAL COMPONENT ANALYSIS (PCA)
We can reduce the number of dimension in large datasets to its principal components which reatain most of the original information. It transforms potentially correlated variables into a smaller set of variables.

Here, we use the module PCA from [sklearn.decomposition](https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html). We will reduce the original 13 features to only two components. This will also allow us to visualize the data in a 2D space.
We obtain well differenciated clusters, which means the PCA worked correctly. But if we analyse closely, we can see that some dots are from the green variable get into the blue and red variable. This overlap suggets that it might be needed more components to distinguish the classes more accurately.

![imagen](https://github.com/user-attachments/assets/54f54855-d1af-4d65-b29d-c9614c520e97)

However, when we run a 

### T-DISTRIBUTED STOCHASTIC NEIGHBOR EMBEDDING (TSNE)
The other method we are working with is TSNE. Just like PCA, it reduces dimensionality in order to interpret better the clusters.
We also use sklearn library for this, the module [manifold](https://scikit-learn.org/stable/modules/generated/sklearn.manifold.TSNE.html).
Just like before, we start by using 2 components.
And we can see how we obtain well differenciated clusters too. And eventhough green class is still messing with the other two, they are more differenciated:
![imagen](https://github.com/user-attachments/assets/53e65003-f24c-43f0-b0ee-b5134e467dfa)







Thanks for reading!

