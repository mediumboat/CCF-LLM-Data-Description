# CCF-LLM-Data-Description
This repository provides data and related descriptions to our CIKM paper "Collaborative Cross-modal Fusion with Large Language Model for Recommendation" https://doi.org/10.1145/3627673.3679596.

# How to obtain the datasets used in our paper

### Raw data

MovieLens-1M: [avaliable here](https://grouplens.org/datasets/movielens/).

Amazon-Books: [avaliable here](https://cseweb.ucsd.edu/~jmcauley/datasets.html#amazon_reviews).

### Data pre-processing

For the MovieLens-1M dataset, the 20 most recent months of user-item interactions are used. The train/validation/test data are split by 10/5/5 months. For the AmazonBook dataset, a total of 16 months of user-item interactions from 2017 onwards are used. The train/validation/test data are split by 11/2.5/2.5 months. In both datasets, users rate items on a 1 to 5 scale. To convert ratings to binary labels, a threshold of 3 is used for MovieLens-1M and 4 is used for Amazon-Book.

Thanks to the authors of [CoLLM](https://arxiv.org/abs/2310.19488) for their contributions. We can obtain the pre-processed dataset from [here](https://github.com/zyang1580/CoLLM/tree/main/collm-datasets).
