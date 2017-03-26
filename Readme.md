
This app is a clone of a simple demo app that has been utilized for the past couple of years.
I have made one major modification to the original app.  The entire tweet is now stored in the CouchDb.  THis will allow me to modify the code in the future so that keyword will become an active link that will pull up the tweets that created the sentiment.


The code consist of a set of node-red flows that arrange the following BlueMix services to create the output.

-Insights for Twitter - to capture Tweets on @Lowes

https://console.ng.bluemix.net/catalog/services/insights-for-twitter?taxonomyNavigation=apps

-Cloudant NOSQL DB - To capture and Store Tweets

https://console.ng.bluemix.net/catalog/services/cloudant-nosql-db?taxonomyNavigation=apps

-Watson Tone Analyzer v3  - To determine the sentiment of keywords in the tweet.  This service ranks keywords as either positive or 
negative and the graph is built based on that output.

https://www.ibm.com/watson/developercloud/tone-analyzer.html

