Project info and results can be found at:


## Data

Download each of the following, and place in the root directory:

* Sample Program Service Data - https://s3.us-east-2.amazonaws.com/datadive-gates92y-seattle/Project+3+-+Form+990+Data/2+-+Clean+Data/Sample_Program_Service_Data.csv

## API keys

In order to get historical tweets, you need share Twitter API secrets.

1. Get a [Twitter Developer Account](https://developer.twitter.com/en/application/)
2. Copy consumer key/secret and app key/secret to `api_keys.json`


## Code

Validated Notebooks:

* `Get the Twitter Handles.ipynb` - Scrape websites (given via Form 990 data) for twitter handles; output to CSV
* `Getting historical tweets.ipynb` - Pulls data from Twitter API. Depends on results from `Get the Twitter Handles.ipynb`. Note: requires Twitter api access (see above for setup)
