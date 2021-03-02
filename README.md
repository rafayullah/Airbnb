# Airbnb Data exploration, analysis and feature engineering
Airbnb, Inc. is an American vacation rental online marketplace company. Airbnb maintains and hosts a marketplace, accessible to consumers on its website or via an app.

The company has attracted criticism for increasing rent prices in cities where it operates. In response, price prediction models, like the one we are going to build here, will help the consumers and company itself to generate alarms if a listing is being made with unjust price.

This project develops a foundation to perform analysis of the data presented by Airbnb. Data from calendar, listings and reviews are processed, visualized and modelled to analyze and predict the price value of the listings. 

The main objective of this project is to demonstrate how the scrapped data can be formulated into features that will help the model to predict the listing's price. You can evolve this project by adding your own set of features using the features utilized by other projects or even features of your own.

# Medium article
https://rafayullah.medium.com/airbnb-data-exploration-analysis-and-feature-engineering-edbb47bf115

## Data

Airbnb Dataset download page:
http://insideairbnb.com/get-the-data.html

The platform hosts updated data of the listings at Airbnb. 
You can use the data from any desired location, this analysis used Boston's data for reference.
Data from multiple locations can be used as well and can be merged using pandas.

As a sample, Boston data is already present under the subfolder './Data'. If you do not want to download your own data, you can use it and skip to the Installation section.


### Here is an example to download and extract data for Boston, USA

Copy the URL of the following: 
* listings.csv.gz
* calendar.csv.gz
* reviews.csv.gz

Copy one of them, follow the steps below and repeat the process for all of the files

#### Download the following datasets using wget:
```bash
cd ./Data
wget http://data.insideairbnb.com/united-states/ma/boston/2020-12-21/data/listings.csv.gz
wget http://data.insideairbnb.com/united-states/ma/boston/2020-12-21/data/calendar.csv.gz
wget http://data.insideairbnb.com/united-states/ma/boston/2020-12-21/data/reviews.csv.gz
```

#### Extract the downloaded datasets using gunzip:
```bash
gunzip listings.csv.gz
gunzip calendar.csv.gz
gunzip reviews.csv.gz
```

## Installation

Python 3 was used for this project.

Install the following Python packages:
```bash
pip install pandas numpy seaborn xgboost spacy spacytextblob
```

Download Spacy Model file:
```bash
python -m spacy download en_core_web_lg
```


## Usage

After the acquisition of data and installation of required libraries, at the root of this project the there will be one python jupyter file and a subfolder in which the data must be present.
To run the notebook, all the cells can be run sequentially, the notebook is segmented into 4 parts:
* Business Understanding
* Data Understanding
* Data Preparation
* Data Modeling
* Evaluation
* Future Improvements


Find below the documentation for Spacy's sentiment analysis library:
Sentiment Analysis Library:
https://spacytextblob.netlify.app/docs/example