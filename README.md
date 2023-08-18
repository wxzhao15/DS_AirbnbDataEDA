# DS_AirbnbDataEDA

## Purpose of this Study

In this analysis, we are using the 2016 Airbnb Seattle dataset provided on Kaggle [link](https://www.kaggle.com/datasets/airbnb/seattle) to better understand the price and availability regarding the airbnb listings and potentially the best neighborhood to choose when visiting. We are focusing on the following questions:
1. How's the listing availability and price looks like throughout the year?
2. What's the best neighborhood to visit in Seattle?

## Data

There are three data sets available. 
(a) listings - 3818 rows, 92 columns: showing what listings are there during 2016, including info such as listing avg reviews, average price, cancellation rule, host info, and other features of listing
(b) reviews - 84,849 rows, 6 columns: contains textual review data along with the review posted date. There are also listing_id and reviewer_id in this dataset that can connect each review to corresponding listing info and reviewer info.
(c) calendar - 1,393,570 rows, 4 columns: this data structure by listing and calendar date to show whether each listing is available on each calendar date in the full time period (2016 Jan ~ 2017 Jan)

In this analysis, we mainly focus on the listings dataset to find insights regarding the price, features, locations and reviews regarding different listings. We also use calendar dataset to analyze how availability and price changes throughout the year.

## Packages

In this analysis, we will use python packages pandas and numpy in Jupyter Notebook to perform data extraction, data trasformation, and data analytics.  

## Analysis Methods

In this analysis, we will be using the CRISP-DM process while analyzing data. CRISP-DM involves multiple steps as listed in the following:
1. Business Understanding
2. Data Understanding
3. Prepare Data
4. Model Data
5. Results
6. Deploy 

## Summary of Results

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
