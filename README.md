# Group Project Team 12482_2

# Dataset

The Netflix - TV Shows and Movies dataset is a comprehensive collection of information on over 6,000 titles available on Netflix in the United States, as of March 2023. The dataset was created using data collected from JustWatch, and is provided in the form of a single CSV file titled titles.csv. The file includes a total of 15 columns of data, which cover a range of important information about each title. These columns include title ID, title name, show type (TV show or movie), description, release year, age certification, runtime (length of episode or movie), genres, production countries, number of seasons (if applicable), IMDB ID, IMDB score, IMDB votes, TMDB popularity, and TMDB score.
 
The titles.csv file provides a detailed overview of the content available on Netflix in the US, with information on each title's genre, release year, and IMDB score. It is a valuable resource for anyone interested in conducting detailed analyses of Netflix's content offerings. Researchers and data analysts can use the dataset to identify popular genres, explore trends over time, or analyze the performance of specific titles. For example, the data could be used to examine how viewership of certain genres has changed over the years or to investigate the factors that contribute to high IMDB scores.
 
The Netflix - TV Shows and Movies dataset is particularly valuable for anyone interested in the entertainment industry or conducting research on media consumption patterns. It provides a rich source of data that can be used to gain insights into the preferences and behaviors of Netflix subscribers. Overall, the dataset is a valuable resource for anyone looking to conduct detailed analyses of the content available on Netflix and to gain insights into the factors that contribute to its popularity.

# Team Members
- [@Grace Fazzone](https://github.com/gracefazzone/graceluvs4610)
- [@Annie Li]()
- [@Young Kim]()
- [@William McBride](https://github.com/WilliamMcB23/MIST4610-Project-2)
 - [@Gustav Bringle]()

## Questions

**1) What are the movie names of the highest IMDB scores across the genres (action, animation, comedy, crime, drama, horror, thriller) and what is the IMDB score variation across each genre?**

An IMDB score is a rating system that is based on user ratings and reviews of a particular film. It provides a useful metric for analysts to evaluate the success of a movie and its general popularity. The score can be influenced by factors such as marketing, movie hype, and the demographic of the users who rate the movie, which are all incredibly useful when analyzing why one movie may have done better than another. That being said, this metric can alter marketing strategy and adjust the release of various movies in order to tailor to movie consumer preferences. 

By splitting each movie by genre and comparing the highest IMDB scores from each, we are able to evaluate a great example of what consumers really like to see in that genre. Furthermore, we can see what the standards and expectations of movies in that genre are and dive deeper into what the other factors each movie had that made it stick out to consumers, whether that be the marketing, demographic, etc. 

Looking at the IMDB score variation across each genre gives us even more insight into this. We can analyze consumer trends and what genres are generally more successful by looking at the median, upper quartile, and lower quartile scores. Netflix is a great source for this data since it is one of the largest streaming platforms in the world with a vast library of content.


**2) What is the range of highest scoring IMDB ratings between production countries and what genres have proven to be hits in some of these highest scoring countries?**

Asking this question helps identify the top performing film production countries and provide insight on personal preferences of people in different regions. Understanding the varying preferences gives invaluable data to optimize planning production strategies. For example, this information can be extremely valuable to interested parties such as filmmakers that want to gain a better understanding of what types of films are likely to be most popular with local audiences.

In addition, analyzing the top genres derived from top IMDB scores helps each country benchmark themselves relative to the global movie market. The different patterns of popular films could be due to a number of things, such as social or cultural differences between countries. Overall, understanding the  genres with high IMDB scores in different countries helps analysts further identify and assess the factors for film success in these countries. Netflix is a great data set to use for this question since Netflix is a global company that operates in over 190 countries worldwide and provides a plethora of genres that include various languages and cultures. 

## Manipulations to Data

There were a few manipulations we had to impose on the data set before we began our data visualization. When we downloaded the data, we noticed that each movie title had many genres and they were all formatted awkwardly. The format had each genre bracketed, with apostrophes surrounding each, and all the genres were in one column together. This made it a bit difficult to grab any real information surrounding the separate genres in our visualizations and we found the extra stuff surrounding the data to look messy. To fix this, we opened the data in Excel and replaced all of the brackets and apostrophes with nothing so it would remove them and make the data look cleaner overall. We then separated each genre by the comma so they were all in separate columns; this allowed us to be able to pivot all of the columns into one genre column and still be able to showcase that each movie can have multiple genres.

Once this was complete,  we ran into an issue in our first visualization where instead of showing us the titles of the movies with the highest IMDB scores, it was returning back every movie title and their IMDB scores. To fix this, we created a calculated field called “MaxTitle” that grabbed only the movie title of each genre that held the top scoring IMDB. We used the LOOKUP and MAX functions to lookup and target the titles with the maximum scores and return that single expression for each of our selected genres.

Finally, for the second question we wanted to look at production countries for each film. In a similar fashion to the problem we ran into with the genre column, the production countries were formatted in a way that aggregated them all into a single column even if there were multiple countries. They also had the brackets and apostrophes surrounding them, so we went through the same process I mentioned earlier in Excel to remove them and separate the countries. We then decided it would be best to just keep the first column of data for ease of use and because we found it an insignificant factor to include multiple production countries for what we wanted to display. 

## Data Visualizations

Question 1:
![Logo](https://github.com/gracefazzone/graceluvs4610/blob/main/Screenshot%20(169).png?raw=true)

![Logo](https://github.com/gracefazzone/graceluvs4610/blob/main/Screenshot%20(170).png?raw=true)

Analysis:

These results ...

Question 2:
![Logo]()

![Logo]()

Analysis: 

These results ...
## Tableau
