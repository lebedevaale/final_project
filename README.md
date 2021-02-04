# final_project
Endembled boosting solution for Predict Future Sales competition on Kaggle

In this solution, you will find an ensemble of the different boosting libraries. Due to several technical limitations (mostly with RAM, which shortened the list of features) and strange bugs (my python doesn't like big pickle files and that's why prepared data is stored in CSV), it is far from being optimal but still looks good.
This notebook will need at least 16 GB of your RAM. The more - the better.
And you would need these libraries to repeat my calculations:
- sklearn
- numpy
- pandas
- matplotlib
- seaborn
- xgboost
- lightgbm
- catboost
I usually use these three libraries for ensembling with the help of a special class, which you find in a notebook. It was modified for time series to fit different validation strategies that need the right order of observations.
Talking about features, I have a list of different combinations of items, their categories, shop types, and subtypes. The only limit sadly was my RAM. In the notebook, you can see some of the features that were cut out not to break calculations.
Also, I should admit that all floats take not less than 32 bytes, just because CatBoost can't work with float16. Honestly, I don't know why it's so, but maybe it will help you to avoid some "magic" mistakes.
