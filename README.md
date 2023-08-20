# Airbnb Seattle 2016 Listings Analysis

## Purpose of this Study

In this analysis, we are using the 2016 Airbnb Seattle dataset provided on Kaggle [link](https://www.kaggle.com/datasets/airbnb/seattle) to better understand the price and availability regarding the airbnb listings and potentially the best neighborhood to choose when visiting. We are focusing on the following questions:  

1. What types of property are listed? How do the price for different property types differ?
2. How's the listing availability and price looks like throughout the year?  
3. What's the best neighborhood to visit in Seattle?  

## Data

There are three data sets available.   
-  listings - 3818 rows, 92 columns:  
   showing what listings are there during 2016, including info such as listing avg reviews, average price, cancellation rule, host info, and other features of listing  

- reviews - 84,849 rows, 6 columns:  
   contains textual review data along with the review posted date. There are also listing_id and reviewer_id in this dataset that can connect each review to corresponding listing info and reviewer info.  

- calendar - 1,393,570 rows, 4 columns:  
   this data structure by listing and calendar date to show whether each listing is available on each calendar date in the full time period (2016 Jan ~ 2017 Jan)  

__In this analysis, we mainly focus on the listings dataset to find insights regarding the price, features, locations and reviews regarding different listings. We also use calendar dataset to analyze how availability and price changes throughout the year.__

## Packages

In this analysis, we will use python packages pandas and numpy in Jupyter Notebook to perform data extraction, data trasformation, and data analytics.  

## Analysis Methods & Findings

In this analysis, we will be using the CRISP-DM process while analyzing data. The CRISP-DM process involves multiple steps as listed in the following:  
1. Business Understanding  

   Understand how does Airbnb operates and get an initial understanding towards the listings. Get to konw some basic quesitons such as the type of property listed, price range, availability 

2. Data Understanding  

   Explore three datasets we have in this project (listing, reviews, calendar). With the datasets we have, we will learn more about hosting side of the operation. With the listing and calendar information we will be able to learn what type of features of listings may be listed at a higher price. But, since we don't have transaction or booking information in this dataset, we are not able to explore the relationship between pricing, booking frequency, return rate hence unable to evaluate the profitability of different listing and its relationship to price and other features.  

3. Prepare Data  

   Since we have 92 columns in listings dataset, a selection of features are chosen to answer each interested business questions. In the process, we will evaluate the missingness of each column and convert data types to suitable one in order to be analyzed. In this process, we have transformed price column from string to numerical, categorical variable "available" in Calendar dataset to dummy variable, cancellation strictness to ordered numerical levels etc.

4. Model Data  
   In the Jupyter Notebook through a series of data cleaning and transformation steps we are able to organize data into a clean analyzable format. In the next, a series of grouping and aggregating will be performed on the cleaned datasets to get to averaged metrics.

5. Results 
   
   1. _What types of property are listed? How do the price for different property types differ? What other findings regarding he property types?_  
      - the most common obsreved property type in this dataset are Houses and Apartments. Together these two types of property are around 90% of all the listings in the dataset.  
      - Boats has highest listed price in the dataset with $285 per night. However, there are only 8 listings are categorized as "Boat" property type. So it might potetntially possess data bias due to its small sample size. But another possibility is due to its limited supply, the market price of it becomes much higher than the others.  
      - 'Dorm' and 'Tent' have lowest price listed at average $35 to $55 range.  

   2. _How's the listing availability and price looks like throughout the year?_  
      - March and holiday season (from October to December) has most listings available on the webstie
      - Price wise, the summer listing averaged highest at around $150 per night. The begning of the year from January to March, the price is the lowest with $120~130 per night.  

   3. _What's the best neighborhood to visit in Seattle?_  
      - Really depends on purpose of the trip, preferred property type and budget. In general, if budget is high and interested in renting the whole house, Queen Anne, Ballard, West Seattle are good areas to explore. There are plenty of listings and high historical location review scores.
      - If interested in renting apartments, among all the area groups, "West Seattle" area rated highest on the location review score (9.79) with averaged listed price per night below $100. If with limited budget but would like to get a good location place, "West Seattle" definitely can be one of the top areas to be considered.

6. Deploy  
   The findings of this analysis is posted on Medium [access link](). 


## License
BSD 3-Clause License

Copyright (c) 2023, wxzhao15

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice,
   this list of conditions and the following disclaimer in the documentation
   and/or other materials provided with the distribution.

3. Neither the name of the copyright holder nor the names of its
   contributors may be used to endorse or promote products derived from
   this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
