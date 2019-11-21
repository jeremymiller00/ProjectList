# ProjectList
A list and basic description of data science projects

## Retrain and Update Manuscript Matcher
Manuscript Matcher takes a manuscript title and abstract and return suggested journals for submission. 
* Created dataset using the last five years of published Title and Abstract from WoS.
* Filtered data down to ~8 million records by removing journals with low publishing frequency and known bad actors.
* Retrained a Fasttext-like FFNN in Tensorflow. Also updated Tensorflow code to enhance forward compatibility.
* Evaluated model using Recall at 1, 5, and 10.
* Performed error analysis based on number of observations by journal.

## Manuscript Prefill - Data Extraction
Given a new manuscript submission, extract and prefill the fields author, title, abstract, institution, funder.

## Add Conflict of Interest by Organization Data to Peer Review Recommendations
Fuzzy comparison of author insstitutions with each potential reviewer institution to idenify potential conflict of interest in peer reviewer recommendation. Comparison made with Jaro-Winkler similarity score. Threshold identified by training a Logistic Regression model with JW as the single feature.

## Predicting Peer Review Suitability for Manuscript Submissions
Given a new manuscript submission to an academic journal, what is the probability of it passing first-line review?
Deep learning FFNN with seven fully connected layers.

## A/B Testing for Reviewer Connect Service
Collect and analyze data from two versions of model to determine statistical differences in results using Bayesian inference.

## Java implementation of RAKE for keyword extraction and TextRank for key sentence extraction  

This project was about halfway completed when I took it over. I have completed the baseline implementations while ensembling a logistic regression model to classify a text token as part of the desired output or not. Since these unsupervised techniques are difficult to evaluate, the next step will be to ensemble a Java implementation of LexRank and use labeled user data to train a supervised ensemble whose features are the scores of the three individual models. 

## Logistic Regression Body Text Classifier.

Written in Scala and trained using Apache Spark. This classifier used part-of-speech tags to classify a given sentence of an academic manuscript as either a "body-text sentence" or not. Precision = 0.90; Recall = 0.90.

## Java implementation of LexRank for extractive summarization

The scores of these three algorithms together form the features of a logistic regression model to rank key sentences for rapid manuscript evaluation.

## Data Reporting Pipeline for Peer Reviewer Recommendation System

Gather, analyze, and present monthly usage data from Reviewer Connect.

## PubMatch Validation

Train logistic regression model to predict if matched publication is desired publication in metadata search. Features are similarity scores of metadata fields (title, abstract, etc..)

## LDA Topic Modeling Proof-of-Concept

Train and visualize Latent Dirichlet Allocation model to identify subtopics in scientific academic publishing.

## Calviz Caltrain future use projection visualization challenge

Worked as part of team to produce a submission to visualize the future ridership and train schedule data under three different funding projections.

## Predicting Success in Online Education

Train Random Forest model to predict final success in online college courses using student interaction data from the first 25% of the course. Metrics:
