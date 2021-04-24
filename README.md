# Toxic Comment Classification Challenge
#### By Lilia BEN BACCAR and Sarah LAUZERAL
### Files
Before explaining the project, here are the description of each file. 
| Python files | Description |
| ------ | ------ |
| `Toxic_comments_classification.ipynb.py` | Project Google Colab |
| `Report.pdf` | Project report |

We have at our disposal a dataset of comments from Wikipedia’s talk page edits. The data folder available on [Kaggle](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/data) is composed by 4 files which are the following:
| Input files | Description |
| ------ | ------ |
| `sample_submission.csv` | a sample submission file in the correct format |
| `train.csv` | the training set, contains comments with their binary labels |
| `test.csv` | the test set, we must predict the toxicity probabilities for these comments |
| `test_labels.csv` | labels for the test data; value of -1 indicates it was not used for scoring |

The test and train are in different files. There are 153164 rows in the test file and we have a train data set of 159 571 Wikipedia comments and 8 columns that are:
  - id
  - comment_text
  - toxic
  - severe_toxic
  - obscene
  - threat
  - insult
  - identity_hate

Each of these comments have been labeled by human raters for toxic behavior. The types of toxicity are the 6 last columns. A single comment can belong to one or more classes and all comments are in english.

The train set comments repartition between the different classes is as follow:
  - toxic		: 15 294 comments
  - severe_toxic	: 1 595 comments
  - obscene	: 8 449 comments
  - threat		: 478 comments
  - insult		: 7 877 comment
  - identity_hate	: 1 405 comments

We will provide a more in depth analysis of how many comments fall into several categories and which categories are the most correlated in our final notebook.

# Context and motivation 
Social media has made it very easy for us to communicate quickly and easily with family, friends and acquaintances, as well as sharing experiences and letting others know of our opinions and beliefs. Our conversations and comments can be closely targeted or widely broadcast to the point that depending on the subject, they can go viral. 

Unfortunately, social media is also widely used by abusers, for exactly the reasons listed above. Many perpetrators ‘hide’ behind the fact that they may not be able to be readily identified, saying things that they wouldn’t consider saying face-to-face, which could be regarded as cowardly. The threat of abuse and harassment online means that many people stop expressing themselves and give up on seeking different opinions. Platforms struggle to effectively facilitate conversations, leading many communities to limit or completely shut down user comments.

# A Kaggle Challenge
Jigsaw and Google have founded Conversation AI team, a research initiative which is working on tools to help improve online conversation. One area of focus is the study of negative online behaviors, like toxic comments (i.e. comments that are rude, disrespectful or otherwise likely to make someone leave a discussion). They’ve built a range of publicly available models but the current models still make errors, and they don’t allow users to select which types of toxicity they’re interested in finding (e.g. some platforms may be fine with profanity, but not with other types of toxic content). 

They decided to create a Kaggle challenge to address this problem. In this competition, we have to build a multi-headed model that’s capable of detecting different types of toxicity like threats, obscenity, insults, and identity-based hate better than Perspective’s current models. The goal is to improve the current model or create another one to hopefully help online discussion become more productive and respectful.

### More explanation
[Click here to go to the Kaggle Challenge](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge)

# References
> Kowsari K, Jafari Meimandi K, Heidarysafa M, Mendu S, Barnes L, Brown D. Text Classification Algorithms: A Survey. Information. 2019

