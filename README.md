# Sentiment-Analysis

Cyber bullying and hate speech has been a menace for quite a long time,So our objective for this task is to detect tweets associated with negative sentiments. From this dataset we classify a tweet as hate speech if it has racist or sexist tweets associated with it.

So our task here is to classify racist and sexist tweets from other tweets and filter them out. With the given twitter dataset consisting of train.csv and test.csv files where we have 31962 labeled tweets. 
The dataset is highly imbalanced.

Sentimental_Analysis_on_twitter_dataset.ipynb contains the code when I did not do anything to deal with the problem of Imbalanced dataset.

## Imbalanced Learning

"The class imbalance problem typically occurs when, in a classification problem, there are many more instances of some classes than others. In such cases, standard classifiers tend to be overwhelmed by the large classes and ignore the small ones."


Sentimental_Analysis_after_Oversampling.ipynb is my notebook where I implemented Oversampling in order to deal with the imbalanced dataset.

#### Through RandomOverSampler the f1_score increased from 0.62 to 0.93 for the minority class (negative tweets).
#### Through SMOTE the f1_score further increased to 0.95.

SMOTE sampling seems to have a slightly higher accuracy and F1 score compared to random oversampling. With the results so far, it seems like choosing SMOTE oversampling is preferable over original or random oversampling.
