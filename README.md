# Delete-favorites-script---Google-Apps-Script

Delete all favorite tweets (unfav) from your account, delete all favorite tweets (unfav) before the last X days.

[Google Apps Script has a limitation](https://developers.google.com/apps-script/guides/services/quotas) on the script runtime of 6 min, so it is advisable to schedule a script execution automatically every 15 minutes so as not to exceed the limits of the Twitter API requests. 

## Prerequisites

**Create new twitter app and configure API**

1. Open Twitter's [Application Management](https://apps.twitter.com/), and create a new Twitter app.
2. Set the permissions of your app to *Read and Write*.
3. Set the required environment variables

**Create new Google Apps Script project [Google Apps Script](https://script.google.com)**

**Copy deleteFavs.gs file in you GAS project and configure variables**

**Execute script and enjoy your life**


## Use

**Configure the following variables:**

```javascript
var TWITTER_USER = 'YOUR TWITTER USER NAME';
var MAX_AGE_IN_DAYS = 30;
var TWEETS_PER_REQUEST = 200;
var CONSUMER_KEY = 'YOUR CONSUMER KEY';
var CONSUMER_SECRET = 'YOUR CONSUMER CONSUMER_SECRET';
var ACCESS_TOKEN = 'YOUR ACCESS TOKEN';
var ACCESS_SECRET = 'YOUR ACCESS SECRET';
```

|variable|description|
|--------|--------------|
|TWITTER\_USER|Twitter username (exclude @)|
|MAX\_AGE\_IN\_DAYS|tweets with a date greater than this number, will be deleted |
|TWEETS\_PER\_REQUEST|Number of tweets per API request |
|CONSUMER\_KEY|The Consumer Key from your Twitter App|
|CONSUMER\_SECRET|The Consumer Secret from your Twitter App|
|ACCESS\_TOKEN|The Access Token from your Twitter App|
|ACCESS\_SECRET|The Access Secret from your Twitter App|


# Versioning

1.0.0

# License

See the [LICENSE](LICENSE.md) file for license rights and limitations (GPL-3).