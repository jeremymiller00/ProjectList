# ProjectList
A list and basic description of data science projects

## Predicting Journal Scope for Manuscript Submissions
Given a new manuscript submission to an academic journal, what is the probability of it passing first-line review?

## A/B Testing for Reviewer Connect Service
Collect and analyze data from two versions of model to determine statistical differences in results

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
