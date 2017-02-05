RedditBotTest
=============

A basic Reddit bot that pulls the 'hot' posts from a collection of dev-related subreddits every 30 minutes and reposts them to a [private sub-reddit](https://www.reddit.com/r/RCBRedditBot/).

To modify, you'll need to register an application on [Reddit's Dev page](https://ssl.reddit.com/prefs/apps) Then, add your clientId, clientSecret, username, and password to a config.js file in the root of the app. ''' // This file is where all app configuration information will go. // It should always be placed in .gitignore so that its contents are not visible to others.

let redditConfig = { clientId: 'YOUR_ID' , clientSecret: 'YOUR_SECRET', username: 'YOUR_USERNAME', password: 'YOUR_PASSWORD' }

module.exports = redditConfig; '''

You will need to add env configs for products or otherwise change how the code handles config data. You SHOULD NOT hard-code your client Secret or user account information!

The app uses [snoowrap](https://github.com/not-an-aardvark/snoowrap) for accessing Reddit's API.

MConstanza
