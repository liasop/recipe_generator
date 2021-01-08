# Recipe Generator and Ingredient Substution

In this project, we use a string of available ingredients, dishes and tags as input, and convert them to a vector representation. We use a word2vec to generate alternative ingredients and recipe names. We also use a recurrent neural network to generate a full recipe including instructions. We hypothesized that our word2vec model should be able to detect ingredients of the same category that are closer to each other (e,g. chicken is more similar to turkey than to coffee), and provides alternative ingredients based on constraints (e.g. the environmental friendly substitute of olive oil is another type of vegetable oil).

The dataset is from Kaggle and the data are from Food.com. Here are a few lines from the dataset

![dataset](https://github.com/liasop/recipe_generator/blob/main/data.png?raw=true)

After creating vector representations of the ingredients, we used TSNE dimensionality reduction to recude the 16D vectors to a 2D space. We then used k-means clustering to find link-ingredients. Here are a couple visuals of the clusterings.

![clusterings](https://github.com/liasop/recipe_generator/blob/main/clust.png?raw=true)

Here are some of our results compared to a baseline dataset: the google news dataset and a google search

![results1](https://github.com/liasop/recipe_generator/blob/main/tab1.png?raw=true)

Here are some of our results compared to a baseline dataset: the google news dataset and a google search

![results1](https://github.com/liasop/recipe_generator/blob/main/tab1.png?raw=true)

Here are some of our results across our different models

![results2](https://github.com/liasop/recipe_generator/blob/main/tab2.png?raw=true)
