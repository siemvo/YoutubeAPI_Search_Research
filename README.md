## YouTube Search Research using YouTube Data API v3
This project utilizes the YouTube Data API v3 to perform search query research using Jupyter Notebooks. The analysis explores various factors affecting video performance, such as video duration, title keywords, subscribers, and tags.

I created this pipeline to do search research to find out how I can optimize video performance in relevant search queries. I collected data from the search queries using the YouTube API and looked into correlations between relevant features and views.

Some important insights I gathered for my specific niche of instrumentals (type beats):
1. Video duration has almost no effect.
When looking at linear correlations between video duration and views, and feature importance in the random forest model, video duration seems to have negligible influence.

2. Video tags are the an important feature importance in random forest regression for predicting views.
It is often thought that video tags do not influence performance as much anymore and the YouTube algorithm works in other ways to recommend videos to users now. The results of my random forest predictions show that video tags are an important feature when taken together. This indicates some form of correlation, but this does not imply causation. When looking at the coefficients for LASSO for individual tags and with some domain knowledge, I would conclude that it is correlation in this situation, but not causation.
