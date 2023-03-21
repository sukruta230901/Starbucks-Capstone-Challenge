# Starbucks-Capstone-Challenge

# Overview
Starbucks, one of the most well-known coffee businesses in the world, routinely gives promotions to consumers through its rewards program to increase sales. These deals may be drink advertisements or may include a discount like a buy one, get one free deal (buy one get one free). The goal of this project is to forecast how customers will react to offers and adapt promotional offers for them depending on how they have responded to previous offers. Exploratory Data Analysis (EDA) is first used to determine the data formats and features to properly evaluate the data. Second, machine learning models are created to forecast how a client will react to an offer, enabling Starbucks to appropriately target the people to whom it makes offers.

# Datasets and Inputs
For this project, the data sets are provided by Starbucks and Udacity in the form of three JSON files. These contains simulated data that mimics customer behavior on the Starbucks rewards mobile app.

* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
* profile.json - demographic data for each customer
* transcript.json - records for transactions, offers received, offers viewed, and offers completed

Here is the schema and explanation of each variable in the files:

**portfolio.json**

* id (string) - offer id
* offer_type (string) - type of offer ie BOGO, discount, informational
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) - time for offer to be open, in days
* channels (list of strings)

**profile.json**

* age (int) - age of the customer
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income

**transcript.json**

* event (str) - record description (ie transaction, offer received, offer viewed, etc.)
* person (str) - customer id
* time (int) - time in hours since start of test. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record

# Libraries Used
* pandas
* numpy
* math
* json
* datetime
* seaborn
* matplotlib
* sklearn
* warnings 

# Files
The following files attached to this GitHub's repository include the following:

* Starbucks_Capstone_Challenge.ipynb: This is the Jupyter Notebook in which I performed all my work.
* proposal.pdf: This document contains the initial project proposal I submitted prior to necessarily beginning this project.
* dataset: This contains the three JSON files provided by Starbucks / Udacity as noted above.
* report.pdf: This document contains a detailed report of the project and describes all the results and observations.

# Acknowledgment
This project was completed as part of Udacity AWS Machine Learning Engineer Nanodegree. The data set provided by Starbucks contains simulated data that mimics customer behavior on the Starbucks rewards mobile app.
