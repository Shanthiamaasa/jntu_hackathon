# Refactored@JNTU - Hackathon - March 2018

Welcome to the JNTU Hackathon. Here are the rules:

* You can work in groups of maximum 3 students per team.
* Each team is allowed just one submission to any one of the 3 problems listed below. Refer to Problem Statements section.
* Points shall be given to those notebooks that have enough explanations, exploratory analysis and
results and most importantly follow the Refactored 5-cell format.
* For reference, go through the lessons on Python, Data Science I at  http://www.refactored.ai.
* You shall use only python for all your programming as that is the industry standard. Any other language notebooks
will not be entertained at this point.
* Once you have completed your analysis, save your notebook and validate it on https://try.refactored.ai before submission.
* Submissions must be made to https://github.com/colaberry/hackathons/jntu-march-2018/ github repository.


## Winner Selection

We shall pick best performing groups amongst the submissions. For reference of best notebooks you can look at:
[Titanic Survival Prediction](https://github.com/colaberry/refactored_labs/blob/master/Titanic-Revisited.ipynb)

You can also learn what steps you need to take to produce such work at:

1. [Python](https://refactored.ai/path/python/)
2. [Data Science I](https://refactored.ai/path/data-science-I/)
3. [Data Science II(Advanced)](https://refactored.ai/path/data-science-II/)

# Problem Statements

We have 3 problem statements for you. You can choose to work on any one of them. Producing a good quality notebook takes time and in our experience, best performing groups have done mostly scored best on solving a single problem with an extensively explained analysis and solution. Here are the 3 problems all of which are equally complex:

## Problem 1: Bitcoin Price Analysis

Historic price of bitcoins are provided for analysis. Your task is to 

1. Ingest the data into a format that is easy for analysis.
2. Perform Exploratory Data Analysis on the dataset.
3. Can you predict the future price of the dataset? 

### 1.1 Time-Series Analysis

Here is an example of time series analysis on Arctic Sea Ice that you can use for your own analysis.

Reference notebook: [Arctic Sea Ice](https://github.com/colaberry/refactored_labs/blob/master/Arctic_Sea_Ice_Analysis.ipynb)

### 1.2 Data Description

[Bitcoin data](https://github.com/colaberry/data/tree/master/Bitcoin)

* Date : Date of observation
* btc_market_price : Average USD market price across major bitcoin exchanges.
* btc_total_bitcoins : The total number of bitcoins that have already been mined.
* btc_market_cap : The total USD value of bitcoin supply in circulation.
* btc_trade_volume : The total USD value of trading volume on major bitcoin exchanges.
* btc_blocks_size : The total size of all block headers and transactions.
* btc_avg_block_size : The average block size in MB.
* btc_n_orphaned_blocks : The total number of blocks mined but ultimately not attached to the main Bitcoin blockchain.
* btc_n_transactions_per_block : The average number of transactions per block.
* btc_median_confirmation_time : The median time for a transaction to be accepted into a mined block.
* btc_hash_rate : The estimated number of tera hashes per second the Bitcoin network is performing.
* btc_difficulty : A relative measure of how difficult it is to find a new block.
* btc_miners_revenue : Total value of coinbase block rewards and transaction fees paid to miners.
* btc_transaction_fees : The total value of all transaction fees paid to miners.
* btc_cost_per_transaction_percent : miners revenue as percentage of the transaction volume.
* btc_cost_per_transaction : miners revenue divided by the number of transactions.
* btc_n_unique_addresses : The total number of unique addresses used on the Bitcoin blockchain.
* btc_n_transactions : The number of daily confirmed Bitcoin transactions.
* btc_n_transactions_total : Total number of transactions.
* btc_n_transactions_excluding_popular : The total number of Bitcoin transactions, excluding the 100 most popular addresses.
* btc_n_transactions_excluding_chains_longer_than_100 : The total number of Bitcoin transactions per day excluding long transaction chains.
* btc_output_volume : The total value of all transaction outputs per day.
* btc_estimated_transaction_volume : The total estimated value of transactions on the Bitcoin blockchain.

### 1.3 Evaluation Criteria:

* Submit the EDA and your solution as a course: 25 points
* Perform prediction of "btc_market_price" on the dataset using regression: 40 points
* Submit to GitHub: 10 points 
* 5 cell format : 20 points + 5 points for Unit testing block
* Level : EDA-Easy, Prediction-Medium 


### 1.4 Naming Convention:

Name your Jupyter notebook file as : 	 TeamID_Bit_Coin		
(replace "TeamID" with the actual ID assigned to your team)


## Problem  2.0 Alpha Solutions Fraud Detection

### 2.1 Overview of Fraud Detection

Fraud is the event of illegal access or execution of a transaction. Fraud modeling is the process where large amounts of transactional data is analyzed to identify observations which do not generally follow the regular patterns. Due to this nature of the problem, anamoly detection and some classification techniques are most suited to analyze such problems and draw valuable insights. More details are available on [wiki](https://en.wikipedia.org/wiki/Data_analysis_techniques_for_fraud_detection):

### 2.2 Problem Statement

A company Alpha solutions provides fraud detection products, solutions and services to financial businesses. One such financial client has many credit card transactions that are provided as the training data. They want the Financial Data Scientist to build models using the available training data. 

![Fraud Model](../images/bayesian_network.png)
<img src="../images/bayesian_network.png", style="width: 800px;">

1. Ingest the data into a format that is easy for analysis.
2. Perform Exploratory Data Analysis on the dataset.
3. Perform classification on the dataset to detect fraud ( logistic regression, naive bayes classifier etc). 

Reference notebook: [Titanic Survival Prediction](https://github.com/colaberry/refactored_labs/blob/master/Titanic-Revisited.ipynb)

### 2.3 Dataset

The data is 10K size samples indicating the categorical variables corresponding to the various categories as shown in the image above.

[fraud data](https://github.com/colaberry/data/blob/master/Fraud/fraud_data.csv)


### 2.4 Evaluation Criteria:

* Submit the EDA and your solution as a course: 25 points
* Perform prediction of "Fraud" on the dataset using classification techniques: 40 points
* Submit to GitHub: 10 points 
* 5 cell format : 20 points + 5 points for Unit testing block
* Level : EDA-Easy, Prediction-Medium

### 2.5 Naming Convention:

Name your Jupyter notebook file as TeamID_Fraud_Detection  (replace "TeamID" with the actual ID assigned to your team)



## Problem 3.0 Air Quality Analysis

All of this data comes from EPA’s Air Quality System (AQS). Data collection agencies report their data to EPA via this system and it calculates several types of aggregate (summary) data for EPA internal use. This includes daily and annual summaries, but not monthly summaries, as these are not routinely needed by EPA. More details can be found at: https://aqs.epa.gov/aqsweb/airdata/FileFormats.html

Refer to the field descriptions at : https://github.com/colaberry/hackathons/blob/master/data/aq_field_descriptions.csv

### 3.1 Problem Statement

1. Ingest the data into a format that is easy for analysis.
2. Perform Exploratory Data Analysis on the dataset.
3. Perform clustering on the dataset to group data based on air quality. 


### 3.2 Dataset

[Air Quality 8 hour sample data](https://raw.githubusercontent.com/colaberry/data/master/8hour_42101_2017_10K.csv)

Reference notebook: [Titanic Survival Prediction](https://github.com/colaberry/refactored_labs/blob/master/Titanic-Revisited.ipynb)

### 3.3 Evaluation Criteria:

* Submit the EDA and your solution as a course: 25 points
* Perform clustering on the dataset using unsupervised learning methods (eg. k-means) : 40 points
* Submit to GitHub: 10 points 
* 5 cell format : 20 points + 5 points for Unit testing block
* Level : EDA-Hard, Prediction-Hard
* Since difficulty level is Hard, your score will be normalized by a scaling factor *1.3


### 3.4 Naming Convention:

Name your Jupyter notebook file as TeamID_Air_Quality (replace "TeamID" with the actual ID assigned to your team)


### Feedback

[Feed back](https://docs.google.com/forms/d/e/1FAIpQLSdD9rpEveAWB8vthGWtFu8GzJhq8U_uxF0zz48Rxn_tzhEQpA/viewform?usp=sf_link)
