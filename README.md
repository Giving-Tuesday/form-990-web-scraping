Project info and results can be found at:


## Data

Download each of the following, and place in the root directory:

* 990 Efile Operational Data 2009 - 2015 - https://s3.us-east-2.amazonaws.com/datadive-gates92y-seattle/Project+3+-+Form+990+Data/2+-+Clean+Data/990Efile+Operational+Data+2009+to+2015.csv
* Data Dictionary - https://s3.us-east-2.amazonaws.com/datadive-gates92y-seattle/Project+3+-+Form+990+Data/2+-+Clean+Data/Data+Dictionary+Project+990+August+2017.xlsx
* Sample Program Service Data - https://s3.us-east-2.amazonaws.com/datadive-gates92y-seattle/Project+3+-+Form+990+Data/2+-+Clean+Data/Sample_Program_Service_Data.csv
* NTEE source: http://nccs.urban.org/classification/national-taxonomy-exempt- entities
* NTEE Classification Data - https://s3.us-east-2.amazonaws.com/datadive-gates92y-seattle/Project+3+-+Form+990+Data/2+-+Clean+Data/NTEE+Classification.csv
* Sample Twitter Data - https://s3.us-east-2.amazonaws.com/datadive-gates92y-seattle/Project+3+-+Form+990+Data/2+-+Clean+Data/giving_tuesday_tweets.csv


## Code

Validated Notebooks:

* `DataCleaningAndClustering.ipynb` - Loads raw form 990 data. Performs some simple cleaning and mapping. Clustering happens in c#, outside the notebook. Cluster results are loaded and viewed.
* `Get the Twitter Handles.ipynb` - Scrape websites (given via Form 990 data) for twitter handles; output to CSV

Need work:

* `Getting historical tweets.ipynb` - Pulls data from Twitter API. Depends on results from `Get the Twitter Handles.ipynb`. Note: requires Twitter api access (see: https://developer.twitter.com/en/application/), with all access secrets added to `api_keys.json`
* `Operational Volatility Analysis-rev.ipynb` - Loads financial data and 990 data; runs financial analytics on them.
