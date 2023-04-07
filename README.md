# ST310-Group-Project
[@BSteiner1](https://github.com/BSteiner1) [@alvaro-dda](https://github.com/alvaro-dda) [@Patrick Braun](https://github.com/patrick-l-braun) [@olly-mapps](https://github.com/olly-mapps) 
 
A coursework project to use Machine Learning on a dataset 

[Stellar Classification Final.pdf](https://github.com/BSteiner1/ST310-Group-Project/files/11178852/Stellar.Classification.Final.pdf)


❓ Questions

**Brief description of dataset:** \
The goal of this project would be to classify a star based on its spectral characteristics. This includes factors such as how "blue" or "red" a star is, or other factors such as redshift.

**Brief description of outcome variable and reasoning for why predicting that outcome (1) makes sense and (2) could produce valuable models:** \
There is a variable class that we can use as our outcome variable. This variable takes categorical values STAR, GALAXY, or QUASAR OBJECT. It could be used in the future to classify newly-identified objects in our solar system.

**Number of observations in dataset:** \
100,000 observations

**Number of variables in dataset available to be used as predictors:** \
There are 18 predictors, but many are identifiers (e.g Object ID) so in reality we have 10 predictors
I think that we can assume that observations are i.i.d. There is one slight caveat to this which is that a determinant of the outcome could be geospatial. It could be the case that there is a higher tendency of one outcome in different regions in our universe. However, this requires a lot of knowledge about this field so probably fine for our use. There is a variable Field_ID which may solve this problem for us. A solution to this problem could be using decision trees to split our observations based on region.

Pros: \
✔️ Lots of clean data \
✔️ Relatively simple to convert qualitative predictors into a qualitative outcome prediction \
✔️ 9 predictors (not too many) means we could use complex methods and it still be computationally feasible.

Cons: \
❌ Almost half of the predictors are identifiers and not characteristics of the object\
❌ Potentially too much data for more complex methods ?\
❌ A high proportion (~60%) of the outcome variable is "GALAXY"
