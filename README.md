# NYU CUSP Capstone 2019
# New York Urban Displacement Project

## Exploring Gentrification and Displacement Through User-Generated Geographic Information

#### Sponsor and mentor: Karen Chapple, UC Berkeley
#### Students: Kent Pan, Tiffany Patafio, Manrique Vargas, Jiawen Wan, Tiancheng Yin

## Table of Contents

1. [Summary](README.md#Summary)
1. [Website](README.md#Website)
1. [Repo directory structure](README.md#Repo-directory-structure)
1. [Introduction](README.md#Introduction)
1. [Modelling](README.md#Modelling)
1. [References](README.md#References)

## Summary

## Website
See the website below:

## Repo directory structure

The directory structure looks like this:

    ├── README.md
    ├── Notebooks
        └── Binary Models
            └── test_1
            |   ├── input
            ├── your-own-test_1


##### 1. Introduction
Our capstone project will study gentrification and displacement risk for neighborhoods within the NY metro region. Using methodology established by the UC Berkeley Urban Displacement Project, and expanding on last year’s CUSP capstone project, we will refine the methodology of the project and expand the scope of the model to incorporate not only administrative census data, but also user-generated social media data (geotagged Twitter data) and other sources of real estate, business, and transportation data. We will use classification models such as random forests with the collected data to better understand granular patterns and variances in activity across changing neighborhoods from those at risk to those in advanced gentrification and exclusion states. With an ever-increasing interest in previously disenfranchised areas as costs within cities climb and investors look for new domain, this area of study is extremely important in helping to shape our cities with residents in mind. The overall goal of our work is to better understand the activities and behaviors in these changing areas so that we can provide insight to help the community, public officials, and other interested parties better manage and plan for the cycle of change. 

##### 2. Modelling
Our goal is to model the typologies defined by last year’s capstone detailed in prior papers using new data sources, including Twitter, Foursquare, and Zillow.  The typologies are inherently divided between high income and low income neighborhoods, which will impact our model design to be similarly split. Our goal, therefore, will be to classify the types of neighborhood change (typologies) undergone in high income and low income areas using our other data sources, Zillow, FourSquare, and Twitter, with the hope of better understanding patterns and activity in neighborhoods across the spectrum of typologies.

We model our problem to output a multiclass classifier of the typologies. The output classifier is represented as y_i, where i corresponds to every census tract in our study. Data pre-processing has been critical to setting a strong foundation for our models. In particular, a large number of possible features in the datasets and a high likelihood for correlation in features required exploration for some feature engineering and dimensionality reduction techniques, such as normalization and regularization, respectively as well as multicollinearity testing. Additionally, handling of categorical variables through factorization will be critical given the frequency of categorical features across datasets. 

Three different models were explored using different features for each dataset, as well as two predictive models, with the target variable being the gentrification typology. Each model was evaluated with four methods: logistic regression, decision trees, support vector machines, and random forests. 

# References
