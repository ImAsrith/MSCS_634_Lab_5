
q Wine Clustering Walk-Through

**Name:** Asrith Krishna Vejandla  
**Course:** MSCS 634 – Advanced Big Data and Data Mining  
**Lab Assignment:** Wine Clustering Walk-Through  

## Purpose of This Lab
In this exercise, I explore how two fundamentally different clustering techniques—Agglomerative Hierarchical Clustering and DBSCAN—segment the classic Wine dataset from scikit-learn. The goal is to gain hands-on experience with both algorithms, understand how parameter choices shape cluster formation, and learn to interpret evaluation metrics and visual outputs in a real-world context.

## Key Insights
When I varied the number of clusters in the hierarchical approach, cutting the dendrogram at three clusters produced a natural separation that closely mirrored the dataset’s true classes. The dendrogram itself served as a powerful visual guide for deciding the most appropriate cluster count. In contrast, DBSCAN shone at identifying noise points, but its performance depended heavily on the `eps` radius and the `min_samples` threshold. A small `eps` treated most points as outliers, while a slightly larger neighborhood radius yielded two clusters with several noise points. Overall, hierarchical clustering offered clearer interpretability, whereas DBSCAN highlighted the dataset’s density variations and outliers.

## Challenges and Decisions
Tuning DBSCAN was part art and part science: I experimented with three parameter sets before landing on values that produced meaningful clusters without overwhelming noise. I also chose to reduce dimensionality to two principal components for plotting, knowing that PCA projections might slightly distort true cluster shapes but greatly improve visual clarity. Finally, I opted for concise, descriptive plot titles and in-cell commentary over boilerplate functions to reflect my own coding style and keep the notebook engaging and original.
