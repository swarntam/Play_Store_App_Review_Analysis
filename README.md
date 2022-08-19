## Overview <Br>
Google Play Store or formerly Android Market, is a digital distribution service developed and operated by Google. It is an official apps store that provides variety content such as apps, books, magazines, music, movies and television programs. It serves an as platform to allow users with 'Google certified' Android operating system devices to donwload applications developed and published on the platform either with a charge or free of cost. With the rapidly growth of Android devices and apps, it was interesting to perform data analysis on the data to obtain valuable insights.


## Problem Statement
The Play Store apps data has enormous potential to drive app-making businesses to success. <br>
**Actionable insights can be drawn** for developers to work on and capture the Android market.<br>Each app (row) has values for catergory, rating, size, and more. Another dataset contains customer reviews of the android apps.<br>**Explore and analyze the data to discover key factors responsible for app engagement and success**

## Data Dictionary <br>
There are two datasets provided for the analysis. The first dataset contains the app-specific information and the other contains the users’ reviews with sentiment analysis. This section explains the features of the datasets provided.

1. Play Store Data <br>
App : The official name of the app on the Play Store. <br>
Category : The category to which the app belongs <br>
Rating : The average rating by the users. <br>
Reviews : The number of reviews the app has received. <br>
Size : The amount of memory required for the app to take space in the phone’s storage. <br>
Installs : The number of times the app has been downloaded. <br>
Type : Binary Values represent whether the app is free or paid. <br>
Price: The price of the app (in US dollars).  0, if free. <br>
Content Rating : Indicates the maturity level of the app for the users. <br>
Genres : Indicates the specific category the app is all about. <br>
Last Updated : The date on which the app was last updated. <br>
Current Ver : The version of the app currently. <br>
Android Ver : The version of Android with which the app is compatible. <br>

2. User Reviews <br>
App : The name of the app. <br>
Translated_Review : Raw text reviews by users <br>
Sentiment : Indicates whether the opinion is positive, negative, or neutral. <br>
Sentiment_Polarity : The strength of opinion in the range [-1,1] <br>
Sentiment_Subjectivity : Measures to what strength a person's opinion is personal. <br>

## Tools used for EDA

1. Numpy : NumPy is a general-purpose array-processing package. It provides a high-performance multidimensional array object and tools for working with these arrays. It is the fundamental package for scientific computing with Python. <br>
2. Pandas : Pandas is an open-source library providing high-performance, easy-to-use data structure and data analysis tools for the Python programming language. It is built on top of NumPy and it steps on its computational abilities <br>
3. Matplotlib : Matplotlib is a plotting library available for the Python programming language as a component of NumPy, a big data numerical handling resource. Matplotlib uses an object-oriented API to embed plots in Python applications. <br>
4. Seaborn : Seaborn is a Python data visualization library built on top of matplotlib. It provides a high-level interface for drawing attractive and informative statistical graphics. <br>
5. Wordcloud : It is a data visualization library widely used for analyzing text data from social network websites. Each text style and size in the visualization indicate its frequency or importance. <br> 

## Table of Contents 
* Problem Statement
* Datasets
* Snapshot of Raw Datasets.
* Setting up the Workspace !
* But why should we do Exploratory Data Analysis ?
* A Quick Look of data we have !
   * Play Store Data
   * Users Reviews
   * Do all apps present in reviews_df are in data_df ?
* Data Wrangling !
   * Checking for duplicates.
   * Missing Values Analysis and Treatment
   * This raises the question Data Quality or Data Quantity ?
   * Data Types Analysis
   * Are all App names unique data_df ?
* Exploratory Data Analysis
   * Play Store Data
     * Rating Variable
     * Free Vs Paid Apps
     * Paid Apps
     * Content Rating
     * Categories wise Analysis
     * Which category has most installed apps ?
     * Does Rating depends on Size of App ?
     * What are unique genres ? What do Genres tell?
     * Pricing Strategies
     * Top Popular Apps
     * Versions
     * What about number of Reviews ?
     * Do people install most reviewd Apps ?
   * Users Reviews
     * Users Sentiments in general.
     * Sentiment Polarity
     * Sentiment Subjectivity
* Combined Analysis
     * User sentiments for free and paid apps.
     * Sentiments across categories.
     * Sentiment Polarity for different sizes.
     * Frequent words in positive and negative sentiments.
* Conclusion
