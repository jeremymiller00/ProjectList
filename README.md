# ProjectList
A list and basic description of data science projects

## Project Currently in Production / Completed
### Retrain and Update Manuscript Matcher
Manuscript Matcher takes a manuscript title and abstract and return suggested journals for submission. 
* Created dataset using the last ten years of published Title and Abstract from WoS.
* Filtered data down to ~13 million records by removing journals with low publishing frequency and known bad actors.
* Retrained a Fasttext-like FFNN in Tensorflow. Also updated Tensorflow code to enhance forward compatibility.
* Evaluated model using Recall at 1, 5, and 10.
* Performed error analysis based on number of observations by journal.
 * This analysis led to the decision to further sample journals with less publications in the dataset.
* Implemented workflow for quarterly model updating and retraining.
* Added PCA 10 dimensional data extaction stage for export to Tableau. The facilitates scope analysis for Publisher Analytics team.

### Ensemble Model for Keyword and Key Sentence Extraction
Java implementation of RAKE for keyword extraction; Java implementations of LexRank and TextRank for key sentence extraction. This project was about halfway completed when I took it over.
* Completed the baseline implementations
* Trained Logistic Regression model in Scala using Apache Spark and Stanford Core NLP to classify a sentence as either "body sentence" or not based on part-of-speech tags.
* Created ensemble linear model using unsupervised algorithm scores and classifier score as features
* Incorporated user feedback data to train ensemble model to improve predictions over time

### PubMatch Validation
Trained logistic regression model to predict if matched publication is in fact desired publication in metadata search. Features are similarity scores of metadata fields (title, abstract, etc..).
* Used to create reports and analsis for Publisher Analytics.

### A/B Testing for Reviewer Connect Service
Collect and analyze data from two versions of Reviewer Connect peer reviewer recommender to determine which is more effective and monitor continuuous performance.
* Use java data extraction tool on ec2 to acquire Reviewer Connect data.
* Performe Bayesian A/B testing by modeling selection rate as a binomial distribution.
* Confirme results of Bayesian A/B testing with traditional Frequentist Hypothesis test.
* Write and deliver reports to stakeholders with test results and plain text description.

### Data Reporting Pipeline for Peer Reviewer Recommendation System
Gather, analyze, and present monthly usage data from Reviewer Connect.
* Worked with Product Manager to define metrics.
* Worked with developers to establish pipeline for data acquisition
* Created and refined data reporting format focusing on visual representations (plots) and plain text descriptions.

## Projects in Development
### Predicting Peer Review Suitability for Manuscript Submissions
Given a new manuscript submission to an academic journal, what is the probability of the manuscript proceeding to Peer Review?
* Produced POC deep learning model based on output of a single, large publisher
* Used Spark, Tensorflow, and Keras

### Add Conflict of Interest by Organization Data to Peer Review Recommendations
Fuzzy comparison of author institutions with each potential reviewer institution to identify potential conflict of interest in peer reviewer recommendation. Comparison made with Jaro-Winkler similarity score. Threshold identified by training a Logistic Regression model with JW as the single feature.

### Author Connect Researcher Search
Given an article or set of articles, find a set of associated researchers.
* A common use case is a journal or conferene that wants to solicit submissions
* Currently this project is worth ~$6mil annually with 3-4k orders per year.
* A human-completed order takes 1-3 hours to complete.

### Manuscript Pre-fill - Data Extraction
Given a new manuscript submission, extract and pre-fill the fields author, title, abstract, institution, funder.

### LDA Topic Modeling Proof-of-Concept
Train and visualize Latent Dirichlet Allocation model to identify subtopics in scientific academic publishing.

### Calviz Caltrain future use projection visualization challenge
Worked as part of team to produce a submission to visualize the future ridership and train schedule data under three different funding projections.

### Predicting Success in Online Education
Train Random Forest model to predict final success in online college courses using student interaction data from the first 25% of the course. Metrics:
