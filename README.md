# ProjectList
An up-to-date list of data science projects with basic description.

## Project Currently in Production / Completed
### Manuscript Matcher - In Production
Helps researchers find the best journals for their work. Manuscript Matcher takes a manuscript title, abstract, and citations as input and returns suggested journals for submission. 
* Created dataset using the last ten years of published Title and Abstract from WoS.
* Filtered data down to ~14 million records by removing journals with low publishing frequency and known bad actors.
* Retrained a Deep Learning in Tensorflow. Also updated Tensorflow code to enhance forward compatibility.
* Evaluated model using Recall at 1, 5, and 10.
* Performed error analysis based on number of observations by journal.
* This analysis led to the decision to further sample journals with less publications in the dataset.
* Implemented workflow for quarterly model updating and retraining.
* Added PCA 10 dimensional data extaction stage for export to Tableau. This dataset facilitates scope analysis for Publisher Analytics team.
* Modified model architecture to make better use of citation data for model inputs.

### Reviewer Connect - In Production
Helps journal editors find peer reviewers for academic manuscript submissions.
* Validated and updated prior model training process.
* A/B testing for Reviewer Connect service: collect and analyze data from two versions of Reviewer Connect.
* Wrote bash script and cron job to automatically extract relevant data from database.
* Perform Bayesian A/B testing by modeling selection rate as a binomial distribution.
* Confirm results of Bayesian A/B testing with traditional Frequentist Hypothesis test.
* Write and deliver reports to stakeholders with test results.
* Work with product manager to perform ad-hoc data analysis to address product team and customer concerns.
* Crafted data reporting pipeline to gather, analyze, and present monthly usage data.
* Worked with Product Manager to define metrics.
* Worked with developers to establish pipeline for data acquisition.

### Ensemble Model for Keyword and Key Sentence Extraction - In Production
In conjunction with other tools, helps editors to quickly assess fit between manuscript and publications. This project was about halfway completed when I took it over.
* Java implementation of RAKE for keyword extraction
* Java implementations of LexRank and TextRank for key sentence extraction. 
* Completed the baseline implementations.
* Trained Logistic Regression model in Scala using Apache Spark and Stanford Core NLP to classify a sentence as either "body sentence" or not based on part-of-speech tags.
* Created ensemble linear model using unsupervised algorithm scores and classifier score as features
* Incorporated user feedback data to train ensemble model to improve predictions over time

### PubMatch Validation - In Production
Matching publisher data to records in Web of Science.
* Trained logistic regression model to predict if matched publication is in fact desired publication in metadata search.
* Used to create reports and analyses for Publisher Analytics.
* Provides insight in rejected manuscripts and representations of published manuscripts.

## Projects in Development
### Author Connect Researcher Search
Given a definition of a research scope, find a set of associated researchers.
* A common use case is a journal or conference that wants to solicit submissions.
* Will augment the current human-researcher driven to reduce costs, fullfill more customer requests, and hopefully increase the click through rates.
* Worked with product team to define metrics and goals.
* Gathered and joined data from mutiple sources to construct training data set.
* Provided POC model with score 50% greater than POC target.
* Worked with subject matter expert to review and validate process and results.
* Aim to be in full production by the end of August 2020.

### Keyword Prediction
Predict match between an academic text and a potential keyword.
* Extracted data set from ~28mil published academic journal articles.
* Trained deep learning model to predict match between text and potential keyword.
* To be used as part of an ensemble for subtopic discovery.

### Predicting Peer Review Suitability for Manuscript Submissions
Given a new manuscript submission to an academic journal, what is the probability of the manuscript proceeding to Peer Review?
* Produced POC deep learning model based on output of a single, large publisher.
* Used Spark, Tensorflow, and Keras.
* On hold due to product team priorities.

### Manuscript Pre-fill - Data Extraction
Given a new manuscript submission, extract and pre-fill the fields author, title, abstract, institution, funder.

### LDA Topic Modeling Proof-of-Concept
Train and visualize Latent Dirichlet Allocation model to identify subtopics in scientific academic publishing.

### Predicting Success in Online Education
Train Random Forest model to predict final success in online college courses using student interaction data from the first 25% of the course.
