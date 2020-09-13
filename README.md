# ProjectList
An up-to-date list of data science projects with basic description.

## Project Currently in Production / Completed
### Deep learning model for ~15,000 class Natural Language classfication problem. Helps researchers find appropriate journals for their work.
* Updated, retrained, and delivered a Deep Learning model with Tensorflow, improving recall@10 by 15%.
* Refactored Tensorflow code to enhance forward compatibility; implemented automated workflow in Databricks for quarterly data updates and model retraining.
* Used Spark SQL to created dataset from rolling 10-year window of published articles.
* Filtered data down to ~14 million records based on criteria determined by consultation with product team.
* Improved model through error analysis to improve predictions from most error-prone inputs; increased recall@10 by 5%.
* Enhanced Publisher Analytics toolkit by implementing PCA data extaction stage for export to Tableau. 
* Aligned product with customer needs by modifying model architecture to account for new features.

### Linear classifier for ranking researcher records. Assists journal editors in finding peer reviewers for academic manuscript submissions.
* Delivered weekly Bayesian A/B testing for old/new model versions over 3 months. 100% of customers moved to new model, with metrics improved by 10% and lower technical debt.
* Wrote bash script and cron job to automate extraction every 2 weeks.
* Delivered monthly data reporting pipeline using Python and SQL to gather, analyze, and present monthly usage data.
* Validated and updated prior model training process.

### Linear classifer for Natual Language document classification. Matches publisher data to company database records for Publisher Analytics reporting.
* Key algorithm in product with revenue ~100k per year.
* Worked with product manager to solicit efficient creation of labeled data set.
* Trained logistic regression model in Python to predict match between publisher and company records; accuracy 96%.
* Wrote and tested basic REST endpoint to provide on-demand predictions.

### Linear ensemble of unsupervised natural language extraction models. Helps journal editors manage workflow by quickly assessing fit between manuscript and publications. 
* Delivered Java implementations of LexRank and TextRank for key sentence extraction. 
* Trained Logistic Regression model in Scala using Apache Spark and Stanford Core NLP to classify candidate sentences.
* Created ensemble model and incorporated user feedback data to improve predictions over time.

### Gradient Boosted Tree / Deep Learning ensemble for combined metadata / NLP regression. Helps journals identify important research, and researchers project their future impact. 
* Delivered POC report showing 15% improvement in MAE over baseline.
* Extracted ~15 million scientific journal articles; performed extensive feature engineering to find predictors.
* Modeled metadata features using a Gradient Boosted Tree model; modeled text content using deep learning; ensembled for best prediction.

### Supervised Word Mover's Distance Python Package
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
