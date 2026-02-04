# Woke-Tweets

**Repository**: [https://github.com/Ray-Aldred/Woke-Tweets](https://github.com/Ray-Aldred/Woke-Tweets)

## Twitter/X Dataset: "Woke" and "Wokeness" Discourse

### Overview

This repository (**Woke-Tweets**) contains tweets scraped from Twitter/X using the search terms **"woke"** and **"wokeness"**. The data was collected on **November 11, 2024** and captures a snapshot of online discourse surrounding these politically and culturally significant terms.

## Dataset Statistics

- **Total Tweets**: 3,000
- **Collection Date**: November 11, 2024
- **Date Range**: November 9-11, 2024 (approximately 2 days)
- **Unique Authors**: 1,569
- **Search Terms**: "woke", "wokeness"

### Tweet Breakdown
- **Original Tweets**: 3,000 (no retweets included)
- **Replies**: 604 (20.1%)
- **Quote Tweets**: 426 (14.2%)
- **Tweets with Media**: 1,593 (53.1%)

## Data Structure

The dataset is stored as a JSON array, with each tweet represented as an object containing the following fields:

### Tweet-Level Fields
- `id`: Unique tweet identifier
- `url`: Link to tweet on x.com
- `twitterUrl`: Link to tweet on twitter.com
- `text`: Tweet text (may be truncated)
- `fullText`: Complete tweet text
- `createdAt`: Timestamp of tweet creation
- `lang`: Language code (primarily "en")
- `source`: Platform/app used to post (e.g., "Twitter for iPhone")

### Engagement Metrics
- `retweetCount`: Number of retweets
- `replyCount`: Number of replies
- `likeCount`: Number of likes
- `quoteCount`: Number of quote tweets
- `viewCount`: Number of views
- `bookmarkCount`: Number of bookmarks

### Tweet Context
- `isReply`: Boolean indicating if tweet is a reply
- `isRetweet`: Boolean indicating if tweet is a retweet
- `isQuote`: Boolean indicating if tweet is a quote tweet
- `inReplyToId`: ID of tweet being replied to (if applicable)
- `inReplyToUserId`: User ID being replied to
- `inReplyToUsername`: Username being replied to
- `conversationId`: ID of conversation thread
- `isPinned`: Boolean indicating if tweet is pinned

### Author Information
Each tweet includes detailed author metadata:
- `userName`: Twitter handle
- `name`: Display name
- `id`: User ID
- `profilePicture`: Profile picture URL
- `coverPicture`: Cover photo URL
- `description`: User bio
- `location`: User-specified location
- `followers`: Follower count
- `following`: Following count
- `createdAt`: Account creation date
- `isVerified`: Legacy verification status
- `isBlueVerified`: Twitter Blue verification status
- `statusesCount`: Total tweets posted
- `mediaCount`: Total media items posted
- `favouritesCount`: Total likes given

### Additional Fields
- `entities`: Contains hashtags, URLs, user mentions, symbols, and timestamps
- `media`: Array of attached media (images, videos)
- `card`: Twitter card data for link previews
- `place`: Geolocation data (if available)
- `extendedEntities`: Extended media information

## Data Collection Methodology

- **Platform**: Twitter/X
- **Filename Convention**: `dataset_tweet-scraper_YYYY-MM-DD_HH-MM-SS-mmm.json`
- **Search Strategy**: Keyword search for "woke" OR "wokeness"
- **Retweets**: Excluded from this dataset
- **Language**: No language filter applied (though dataset is primarily English)

## Potential Use Cases

This dataset can be used for various analytical purposes:

1. **Discourse Analysis**: Examining how terms "woke" and "wokeness" are used in online political discourse
2. **Sentiment Analysis**: Understanding the emotional tone and polarity of discussions
3. **Network Analysis**: Mapping conversation patterns and influential users
4. **Temporal Analysis**: Tracking how discourse evolves over the collection period
5. **Political Communication**: Studying political messaging and framing strategies
6. **Linguistic Analysis**: Examining language patterns, hashtag usage, and co-occurring terms
7. **Media Analysis**: Analyzing the role of images and videos in these discussions
8. **Engagement Patterns**: Understanding what content generates the most interaction

## Data Quality Considerations

- The dataset represents a **sample** of tweets, not a comprehensive collection of all tweets containing these terms
- Tweet availability depends on user privacy settings and account status at time of collection
- Some tweets may have been deleted or made private since collection
- Engagement metrics (likes, retweets, etc.) are snapshots from the collection time and may have changed
- The dataset may be influenced by Twitter/X's search algorithm and ranking

## Ethical Considerations

When working with this dataset, researchers should consider:

- **Privacy**: While tweets are public, consider the ethical implications of analyzing user data
- **Context**: The terms "woke" and "wokeness" are politically charged and contextually dependent
- **Bias**: The dataset reflects Twitter/X's user base and may not represent broader public opinion
- **Sensitivity**: Discussions may contain controversial political content
- **Informed Consent**: Users may not have expected their tweets to be part of research datasets

## File Information

- **Filename**: `dataset_tweet-scraper_2024-11-11_23-29-36-565.json`
- **Format**: JSON (JavaScript Object Notation)
- **Size**: ~823,475 lines
- **Encoding**: UTF-8

## Recommended Analysis Tools

- **Python**: pandas, tweepy, nltk, scikit-learn
- **R**: rtweet, tidyverse, quanteda
- **Visualization**: matplotlib, seaborn, ggplot2, Tableau
- **Network Analysis**: NetworkX, igraph, Gephi
- **Text Analysis**: spaCy, NLTK, TextBlob, VADER

**Dataset Details**:
- Repository: Woke-Tweets
- Collection date: November 11, 2024
- Search terms: "woke", "wokeness"
- Platform: Twitter/X
- Date range: November 9-11, 2024

## Version History

- **v1.0** (2024-11-11): Initial collection of 3,000 tweets

## Contact and Updates

- **Repository**: [https://github.com/Ray-Aldred/Woke-Tweets](https://github.com/Ray-Aldred/Woke-Tweets)
- **Issues**: For questions about this dataset or to report issues, please open an issue on GitHub
- **Maintainer**: Ray-Aldred

---

*Last Updated: November 11, 2024*
