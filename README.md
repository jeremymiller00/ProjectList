# ProjectList
An up-to-date list of data science projects with basic description.

## Project Currently in Production / Completed
### Manuscript Matcher - In Production
Helps researchers find the best journals for their work. Manuscript Matcher takes a manuscript title, abstract, and citations as input and returns suggested journals for submission. 
* Used Spark to created dataset using rolling 10-year window of published articles from WoS.
* Filtered data down to ~14 million records by removing journals based on criteria determined by consultation with product team.
* Retrained and delivered a Deep Learning model with Tensorflow. Model metrics improved by 18%.
* Updated Tensorflow code to enhance forward compatibility; implemented workflow for quarterly data updating and model retraining.
* Improved model through error analysis to improve predictions from most error-prone inputs.
* Enhanced Publisher Analytics toolkit by implementing PCA data extaction stage for export to Tableau. 
* Aligned product with customer needs by modifying model architecture to account for new features.

### Reviewer Connect - In Production
Helps journal editors find peer reviewers for academic manuscript submissions. 
* Validated and updated prior model training process; identified opportunity for model updating based on data source.
* Delivered Bayesian A/B testing for old/new model versions. 100% of customers moved to new model, with metrics improved by 10% and lower technical debt.
* Wrote bash script and cron job to automate extraction of relevant data from database, facilitating ongoing testing.
* Crafted data reporting pipeline using Python and SQL to gather, analyze, and present monthly usage data.

### Ensemble Model for Keyword and Key Sentence Extraction - In Production
In conjunction with other tools, helps editors to quickly assess fit between manuscript and publications.
* Delivered Java implementations of LexRank and TextRank for key sentence extraction. 
* Trained Logistic Regression model in Scala using Apache Spark and Stanford Core NLP to classify candidate sentences.
* Created ensemble model and incorporated user feedback data to improve predictions over time.

### PubMatch Validation - In Production
Matching publisher data to records in Web of Science. Used to create reports and analyses for Publisher Analytics.
* Worked with product manager to solicit efficient creation of labeled data set.
* Trained logistic regression model in Python to predict if matched publication is in fact desired publication in metadata search.
* Wrote and tested basic REST endpoint to provide on-demand predictions.
* Key algorithm in product with revenue ~100k per year.

### Citation Count Prediction - POC
At the time of publication, predict citation count for scientific journal articles 3 years after publication. Helps journals and editors identify important research. Helps researchers project their future impact.
* Extracted ~15 million scientific journal articles.
* Extensive feature engineering to find predictors.
* Modeled metadata features using a Gradient Boosted Tree model; modeled text content using deep learning.
* Modeling initially done separately to understand relative predictive power of each.
* Ensemble of two models provides best scores.
* POC report delivered to product manager for assessment of further work.

### Supervised Word Mover's Distance
A technique for using document labels to transform word-vector space such that documents with matching labels are close togehter.
* Wrote Python package to implement Supervised Word Mover's Distance.
* Useful for measuring document distance when a particular dimension is of interest.
* Available for use throughout company.

## Projects in Development
### Author Connect Researcher Search
Given a definition of a research scope, find a set of associated researchers. Typical use case is a journal or conference that wants to solicit submissions.
* Will augment the current human-researcher driven to reduce costs, fullfill more customer requests, and hopefully increase the click through rates.
* Worked with product team to define metrics and goals.
* Gathered and joined data from mutiple sources to construct training data set.
* Trained Gradient Boosted Tree model with Spark ML.
* Provided POC model with score 50% greater than POC target.
* Worked with subject matter expert to review and validate process and results.
* On schedule to be in full production by the end of August 2020.

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
