# RBMrecommend
RBMrecommend is a recommender system predicting user's inclination toward unknown items with Restrictive Boltzmann Machine (RBM). RBM recommend is trained with a dataset of users' browsing history. A user expressed like or dislike to few random items in the market while the rest items remain unknown to the user, and RBMrecommend collaboratively filters out other unwanted items based on similar users' preferences.

For personal learning purpose, this project is a miniature version of Restrictive Boltzmann Machine recommender ([Salakhutdinov et al., 2007](https://www.cs.toronto.edu/~rsalakhu/papers/rbmcf.pdf)), which was in the leading position in the [Netflix prize](https://www.netflixprize.com/). An introduction of RBM can be found in my other project [RBMIsing](https://colab.research.google.com/drive/1kEoVz9gX-RKd6VXEmARyT5RmSOA1ah3q#scrollTo=gf3xHXYRou0M).

The input data is a user-item matrix with entries = (1, 0, NaN) for like, dislike, and unknown items respectively. The dataset is generated artificially, so one can easily experiment with various trends of customers/items. For demonstration, presented data consists of 2,000 customers and 100 items. Training data records random twenty like or dislike items for every customer, and the rest items are marked unknown. 

This project is written in Python 3.0 and demonstrated on Google colab. The training takes less than half a minute for 2000x100 user-item dataset, and the prediction accuracy is about 80+%.



