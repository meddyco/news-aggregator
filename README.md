# News Aggregator

### Description 
For this assignment you have to implement an application that aggregates news from two different APIs. The APIs you'll be using are [Reddit](https://www.reddit.com/dev/api/ "Reddit") and [News API](https://newsapi.org/ "News API"). This application should be running on your localhost and serve the result in JSON format from an endpoint whenever it gets a request. The two functionalities that need to be implemented are "list" and "search".

This is an example request for a generic GET request.

```
> Request
GET /news   HTTP/1.1
Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ
Accept: application/json

> Response
[
  {
    "headline": "Human organs can be stored for three times as long in major breakthrough for transplants",  // Headline of the article
    "link": "https://www.telegraph.co.uk/science/2019/09/09/human-organs-can-stored-three-times-long-major-breakthrough/",  // Link of the article
    "source": "reddit" // Source that you retrieved this news from
  },
  {
    "headline": "Depth of Field: The Shared Memory of One World Trade Center",
    "link": "https://www.wired.com/story/one-world-trade-center-history-future/",
    "source": "newsapi"
  },
]
```

You should also implement a feature that allows someone to search.

```
> Request
GET /news?query=bitcoin   HTTP/1.1
Authorization: Basic QWxhZGRpbjpvcGVuIHNlc2FtZQ
Accept: application/json

> Response
[
  {
    "headline": "IRS goes after cryptocurrency owners for unpaid taxes",
    "link": "https://www.cbsnews.com/news/own-bitcoin-irs-pursues-cryptocurrency-owners-for-unpaid-taxes/",
    "source": "reddit"
  },
  {
    "headline": "Skirting US sanctions, Cubans flock to cryptocurrency to shop online, send funds",
    "link": "https://www.channelnewsasia.com/news/business/skirting-us-sanctions--cubans-flock-to-cryptocurrency-to-shop-online--send-funds-11901148",
    "source": "newsapi"
  },
]
```

*Suggestion:* Try to use /r/news for Reddit and the general category for News API (you don't have to but it's worth checking out).

The application that you submit must have thoughtful design decisions, well documented and unit tested code. This assignment should not take more than 5 hours to complete.

### Constraints
You have to use **Python**, however, you can use any framework or library you're most comfortable with.

You have to return the three fields that are in the sample requests above! You can add more fields if you'd like.

This needs to be a running Python application on your localhost that serves an HTTP request not a console application.

### Submission
You should upload your code to a Github repository (private or public) and share it with me. Your repository should have a README.md that explains how to run the code and if you’ve done anything extra. If you fail to produce this repository within the time period mentioned in the email you received your application will be rejected.

### Assessment
This assignment is meant to test:
- Proficiency with Python
- Ability to understand and use 3rd party APIs
- Ability to parse different forms of data
- Abilty to use Github
- Ability to write unit tests
- Ability to write documentation

What I will be looking for:
- Great code design and architecture that is extendible to more 3rd party news apps or more fields
- Well documented clean code with unit test
- Clean commit history that reveal the evolution of this application

Best of luck!

~ Meddy Team


