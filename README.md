White Wind Quality Prediction Model

This repository is for the creation of a machine learngin model to predict the rating of white wines.

The model I am choosing for production is a RandomForestClassifier at a depth of 17. It has the highest accuracy of all the models, tied only with a GridSearch KNN model. However, this model is much less compuationally taxing and much faster to run.
![final model](https://user-images.githubusercontent.com/101794920/176862844-f1948918-621a-4213-b152-14b08c22993a.JPG)



There are some issues that should be kept in mind when using this model. While it is most accurate on determing the quality rating of mid level wines, 5-7, it should not be used for wines of high quality, 8-10. This can be improved by adding more high quality wines to the dataset.

Additionally, the data set had many features that were two measures of a similar chemical properity, with 3 measure for acidity and 2 measures for sulpher dioxide. Adding more varied features, such as tannin levels or grape variety used, would improve the models perfomance. The data set also includes only white variants of the Portuguese "Vinho Verde" wine. Including white wines from other regions, or included red winse from the same region, would also be a good choice from providing a more robust data set for the model.

