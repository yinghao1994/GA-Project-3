# Project 3: Battle of the Dating Apps - CoffeeMeetsBagel v.s. OkCupid
#### Don Chng, General Assembly SG-DSI-14
#### 17th May, 2020



## Background Information 

Some of the most downloaded dating apps include Tinder, Bumble, CoffeeMeetsBagel, OkCupid etc. Ever since the advent of dating apps, dating service companies have been trying to outdo each other in terms of app subscribtions, as well as onboarding premium subscribers. Especially over the past few years, we have seen an influx of more dating apps which offers comparably different matching methodologies and algorithms. According to statistia.com, revenue in the online dating segments amounts to around 1.7 billion USD per year, with a projected annual growth rate of 9.3% in the next 3 years.

The onling dating apps industry still proves to be a popular investment choice for both venture capitalists and angel investors. Our clients, Venus Dating Pte Ltd, is a new start-up that seeks to penetrate into the dating app scene and has hired us as data science consultants to conduct basic data anaylsis on their competitors.

For a start, our team is focusing on two companies for the inital research, CoffeeMeetsBagel and OkCupid. We plan to scrape data from reddit, a popular online forum where netizens gather to discuss about the latest social news and trends. In this instance, reddit would be the perfect platform to find out what people's perception of these dating apps are. Natural Language Processing will be used to analyse the posts, and a model will be built to classify posts form the two different apps, using key words as the features in the model.

## Problem Statement

It is important to identify key trending words and phrases in these subreddit posts for dating apps, as the general themes of discussion can give us key insights on how people perceive an online dating site to be. Furthermore, we would want to build a classifier using these key words as features of model, in order to verify whether the words are indeed representative of themes revolving around a dating app. The **accuracy score** would be used to determine the performance of the classifier model. 


## Modelling

Multinomial Naive Bias Classifier and Logistic Regression were both used to classify these text. Multinomial NB has shown to have the best performance, via using CountVectorizer. 

## Conclusion


### Summary
Even though CMB and OKC are similar with their purpose as a dating app, they are different in terms of the way matchmaking is done. To provide a rough context, CMB sends its male counterparts ( a.k.a coffee) 21 profiles of females (a.k.a bagels) per day, which is a fairly limited amount compared to other apps. As for OKC, males and females are able to view each other's profile freely and it is unlimited.

CMB's subreddit most used words seem to be focused on the subject of profile and matches. A good reason for this would be that since CMB has limited the number of profile views for guys per day, a huge concern for the CMB community would be placed on creating quality profiles and getting quality matches. A dominant issue in the dating app industry is that some people use dating apps only for casual relationships, while others might be seeking more serious relationships. According to an article from techcrunch.com, CMB "puts more emphasis on user profiles", since you only have a limited number of matches per day, it encourages the user to glean more information on the other person before coming to a decision. This is very unlike other dating apps like Tinder, where people would accept or reject a profile mostly based on the profile picture.

As for OkCupid, words like "feel" and "dating" are more prominent. Just from glancing through the nature of the subreddit contents in OKC, alot of these posts are more focused on their dating experiences with their counterpart, once they have matched in OKC. "Profile" is also ranked quite highly as OkCupid also places emphasis for users to create a profile representative of themselves.

The models generated have managed to obtain a high rate of accuracy in classifying the posts. This shows that the vectorizers such as Count and TF-IDF have done well in filtering out keywords that are peculiar for the dating app. In summary, CMB users seem to be having more focused discussions on profiling and matching, while OkCupid users are more focused on sharing their dating experiences in the reddit forums.

### Limitations
From the word cloud rankings, we notice that OkCupid has words like '2020','quarantine', 'coronavirus' and 'april'. These words refer to the current period we are in, and the coronavirus is a worldwide pandemic that is currently happening in April 2020. Since the web-scraped search results were taken from the latest subreddit posts, OkCupid has many more posts mentioning current events like the coronarvirus and quarantine situations, whereas for CMB, there was lesser mention of these current events.

What we can possibly infer from this information is that OkCupid's subreddit has a much more active userbase than CMB. As a matter of fact, OkCupid has about 200,000 members, whereas CMB has only 7,300 members up to date. With a more active base on OkCupid than CMB, getting new information on trends based on the CMB's subreddits maybe be comparatively slower than OkCupid.

### Recommendations
These types of information are very telling in identifying the unique selling points (USP) of the different dating apps, as well as to monitor the perceptions from the netizens about these dating apps. CMB focuses more on quality matches for both partners, leading to serious relationships. OkCupid might be more focused on the experience of using the app for dates itself. For our clients, Venus Dating, they would want to take these different USPs into consideration and create a selling proposition that will allow them to penetrate the already saturated dating app market.

More research can be definitely conducted on reviews of the app itself on platforms such as Apple Store and Google Play, where users will usually rate the app out of a given score of 5, and leave any remarks about their satisfaction of the product. It may be also useful to glean on data written on blog reviews, as these platforms tend to be much more verbal and thought out than a passing comment in reddit or an online app store.