## RatBot
A bot thath scoope subredits and repost his content on twitter

**Features:**

* Can post to both Twitter 
* Runs in the cloud with a free Heroku account, or locally on any PC with Python
* Media from direct links, Gfycat, Imgur, Reddit, and Giphy is automatically attached in the social media post
* Links that do not contain media can be skipped, ideal for meme accounts
* NSFW content, spoilers, and self-posts can be filtered
* Multiple subreddits can be monitored at once

Ratbot uses the [tweepy](https://github.com/tweepy/tweepy), [PRAW](https://praw.readthedocs.io/en/latest/), [py-gfycat](https://github.com/ankeshanand/py-gfycat), [imgurpython](https://github.com/Imgur/imgurpython), [Pillow](https://github.com/python-pillow/Pillow).

## Setup and usage
**Install the dependences**

```bash
pip3 install requirements.txt
```
**Using the config file**
* 1. Under the [BotSettings] section, add the name of the subreddit to SubredditToMonitor (do not include the /r/). You can also set multiple subreddits using the + symbol (example: AnimalsBeingBros+babyelephantgifs+aww).
* 2. By default, the bot will wait at least 600 seconds between tweets to prevent spamming. You can change this by editing the DelayBetweenTweets setting in the [BotSettings] section.
* 3. By default, the bot will only look at the top 10 'hot' posts in a subreddit. You can change this by editing the PostLimit setting in the [BotSettings] section.
* 4. You can enable or disable NSFW posts and self-posts, by changing NSFWPostsAllowed and SelfPostsAllowed to true or false.
* 5. If you want Tootbot to only post media (images, GIFs, GIFV files, etc), set MediaPostsOnly to true.

**Entering API information**
Next, you need to run Tootbot to setup API access with Reddit, Imgur and Twitter
Open the command line/terminal and set your directory to the Tootbot folder. Then type this command:

```bash
python3 ratbot.py
```
After Tootbot starts up, it will begin asking for API keys. You only have to do this process once.

**AND U HAVE IT RUNNING**
