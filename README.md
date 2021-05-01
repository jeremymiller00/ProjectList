# ProjectList
An up-to-date list of data science projects with basic description.

## Project Currently in Production / Completed
### Custom Java Library for Bespoke Term Extraction Use Case from Patent Document Database.
* Worked with team members to define requirements and test cases.
* Designed and executed expert review process to ensure quality output.
* Delivered production Java 8 library with full test coverage.

### Deep learning model for ~15,000 class Natural Language classfication problem. Helps researchers find appropriate journals for their work.
* Updated, retrained, and delivered a Deep Learning model with Tensorflow, improving recall@10 by 15%.
* Refactored Tensorflow code to enhance forward compatibility; implemented automated workflow in Databricks for quarterly data updates and model retraining.
* Used Spark SQL to created dataset from rolling 10-year window of published articles.
* Filtered data down to ~14 million records based on criteria determined by consultation with product team.
* Improved model through error analysis to improve predictions from most error-prone inputs.
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
* Trained logistic regression model in Python to predict match between publisher and company records; accuracy 99%.
* Wrote and tested basic REST endpoint to provide on-demand predictions.

### Gradient Boosted Tree model for metadata classification. Finds relevant researchers for email marketing product.
* Projected to decrease product delivery time by at least 50% for product with ~6mil annual revenue.
* Delivered Gradient Boosted Tree model with Spark ML with score 50% greater than POC target.
* Worked with product team to define metrics and goals.
* Gathered and joined data from mutiple sources to construct training data set.
* Worked with subject matter expert to review and validate process and results.

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

## Projects in Development / Prototypes
### Document Cluster Label Extraction / Creation
* Given a cluster of related documents ranging in size from approximately 10 to 10,000, extract / create a meaningful, "readable" label for users.

### Keyword Prediction
Deep Learning Natural Language token classification. Predict match between an academic text and a potential keyword.
* Extracted data set from ~28mil published academic journal articles.
* Trained deep learning model to predict match between text and potential keyword with AUC 0.96.
* To be used as part of an ensemble for subtopic discovery.

### Predicting Peer Review Suitability for Manuscript Submissions
Given a new manuscript submission to an academic journal, what is the probability of the manuscript proceeding to Peer Review?
* Produced POC deep learning model based on output of a single, large publisher with AUC 0.82 and Area Under P/R Curve 0.87.
* Used Spark, Tensorflow, and Keras.
* On hold due to product team priorities.

### LDA Topic Modeling Proof-of-Concept
Train and visualize Latent Dirichlet Allocation model to identify subtopics in scientific academic publishing.

### Predicting Success in Online Education
Train Random Forest model to predict final success in online college courses using student interaction data from the first 25% of the course.
