 ![images](https://user-images.githubusercontent.com/125798275/224466315-95e1a969-2404-4368-9c05-9146f88e8dc0.png)

 PROJECT LINK - https://fuzzy-melons-unite-35-230-0-106.loca.lt/

     
     What is Twitter Scraping?
Scraping is a technique to get information from Social Network sites. Scraping Twitter can yield many insights into sentiments, opinions and social media trends. Analysing tweets, shares, likes, URLs and interests is a powerful way to derive insight into public conversations. It is legal to scrape Twitter or any other SNS(Social Networking Sites) to extract publicly available information, but you should be aware that the data extracted might contain personal data

Scraping can be done with the help of many opensource libraries like
Tweepy,
Twint,
Snscrape,
Getoldtweets3
For my project I have used SNSCRAPE library.

Libraries and Modules needed for the project!
snscrape.modules.twitter - (To Scrape the Data from Twitter)
Pandas - (To Create a DataFrame with the scraped data)
Pymongo - (To upload the dataframe to MongoDB database)
Streamlit - (To Create Graphical user Interface)
Datetime - (To get the current date)

Acknowledgements
GUVI,
Mentor Mr.Nethaji Nirmal,
Streamlit docs.


Scraping the tweet
To scrap the data Snscrape python library is used. The TweetSearchScrape() method scrape the Twitter data without Twitter API. The method is passed with a query conating the hashtag to be search and the search dates (From start date to end date)

Uploading data in MongoDB
Tweets that are scraped using the Snscrape library is inserted into the MongoDB database by establishing the clinet connection. The tweet datas are strored under the twitter db collections.
Creating the UI
Used Streamlit app for creating the GUI for Twitter Scraping. Used menus for searching, dispalying the tweets and to download.

Menu 1 -- Home
Home page of the UI conatins title of the app

Menu 2 -- About
Conatins small description about the Twitter Scraping, Snscrape librray, MongoDB and Streamlit framework.

Menu 3 -- Search
Search menu which is used to search the tweet data usng the #hashtag and for given dates. Everytime the search menu deletes the existing datas while searching the new tweet in order to retrive the tweet information correctly.

Menu 4 -- Display
The scraped data from the MongoDB database are dispalyed as a DataFrame

Menu 5 -- Download
The scraped data from the MongoDB database is downloaded as CSV/ JSON file formats as per the requirement.
