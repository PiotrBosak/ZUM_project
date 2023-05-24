## Introduction

This is a project that analyzes sentiment of comments from forums dedicated to different music genres.
It tries to answer the question of how music fans, across different genres, express thoughts and discuss their favorite artists or albums.

## Data collection

Scraped data are comments from 5 different subreddits dedicated to specific music genre(hip hop, classical, metal, punk, jazz).
The data was scraped using `snscrape`, for each genre there is 100k-150k comments(500k-600k in total), although not all rows are actually used(see the next section).

## Initial project's vision and techniclal obstacles

Our initial idea for this project was to collect data from multiple formus and then compare the sentiment of comments among different music genres.
Volume of the scraped data does allow for such a comparison, however Google collab's resource limits do not.
Google collab can only handle ~30k rows when training our models.
Using personal laptops was also not feasible as many Python libraries do not work on ARM processors.
Splitting the data between different genres would mean few rows per model, too few to properly train the networks.
We ended up merging the scraped data and therefore changing the project's goal: sentiment analysis of comments in forums dedicated to music.
While different from the original, we believe the project's goal is still a valid and an interesting one.


## How to use it

This project was created using Google collab.
The `.ipnyb` notebooks present in this repository assume the required inputs are on the user's Google drive.
The outputs will be either saved on the user's Google drive or displayed inside the notebook.

The projects contains:
- ZUM_classic_neural.ipynb: this file contains data collection, classic ML and neural ML stages.
- ZUM_BERT.ipynb: contains BERT language model
- ZUM_hugging_face_zero_shot.ipynb.ipynb: contains hugging face zero shot model


## Project doumentation
Each part of the project is documented inside the notebook, please refer to it for explanations of implementation details and the results' analysis.


## Authors
While there's only one commiter in the repository, this project was created collectively by:
Piotr Bosak - s18692
Piotr Zaborowski - s18665
Mateusz Kozłowski - s18541

