# FTX Dogecoin bot powered buy Elon Musk on Twitter 

FTX-ELON-TWITTER-DOGE-BOT is a python script which monitor Elon Musk twitter feed for "Dogecoin" mention buy some coin before automatically selling it.

*Be aware that this script is for educational purposes only, by an idea of antoinebaron-io*

The script will open a stream connection to twitter API and monitor Elon Musk twitter account.
If a mention of dogecoin is found in his last tweet, the script will immediately request a convert order from your USD balance and automatically convert it back to USD after 20 minutes.
The script will also writed down in a Gsheet document every action so you know how much USD you made at the end of the convert process.

![alt text](https://imgur.com/a/RZ47sB9)

## Dependencies

- API key from your FTX account (https://ftx.com/profile)
- API key from twitter developer (https://developer.twitter.com/en/apply-for-access)
- Google Gsheet API and service_account created with JSON creds (https://developers.google.com/workspace/guides/create-project)

The script works using : 
- Tweepy : https://docs.tweepy.org/en/stable/
- Gspread : https://docs.gspread.org/en/latest/
- FTX API : https://docs.ftx.com/#overview

## Installation

>pip3 install tweepy, gspread, requests

## Configuration

You have to store your Twitter and FTX API credentials into the .dev file and download your Google service_account.json file.

## Usage

Create a new file index.php and paste :

>python3.8 ./twitter_stream.py

----------------------------------------------------------------------------------------
