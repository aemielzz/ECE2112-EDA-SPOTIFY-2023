## ECE2112-EDA-SPOTIFY-2023
### PYTHON DATA ANALYSIS (PANDAS)
##### Amiel Elestin M. Cruz
##### 2ECE-D

![image](https://github.com/user-attachments/assets/a91c5005-efbf-4bc6-9661-b0aa9157c1c8)

When using numbers, and grap it is mandatory to input "Import pandas as pd","Import matplotlib.pyplot as plt","Import seaborn as sns" to access pandas lib and to display graphical infromation.

![image](https://github.com/user-attachments/assets/b6149786-1bf7-40be-bcea-fd83bf5bc1b6)

I named the data as spoti. and I used pd.read to display the overview the data set.

## Overview of Data set

#### How many rows and columns does the dataset contain?
#### What are the data types of each column? Are there any missing values?

![image](https://github.com/user-attachments/assets/ee1511aa-0b2c-4919-bde2-5939263fe714)

As we can see there are 953 rows and 24 columns. We can also see the different types of Data in the table. 

![image](https://github.com/user-attachments/assets/ee282fa3-be52-4e85-9de0-f659a6bfe3b5)

As we can see from the image above, the code showed the missing values asked in the guide questions.



## Basic Descriptive Statistics

#### What are the mean, median, and standard deviation of the streams column?
![image](https://github.com/user-attachments/assets/e8967669-f6cf-4f93-9ab5-3eb86f777b5f)

we declared the code for different uses, I used the pd.to_numeric(): to conver the data into numbers and  spoti['streams']: because I want to get the mean median and mode on the stream column and errors='coerce': for panda to not cause an error in data that are not numbers and display NaN
. as we get the mean of the streams column we used again the  spoti['streams'].mean to solve for the mean and we named that data as "mean", we just repeat the following and just replace the mean as median and standard deviation to automatically solve for the median and std.

#### What is the distribution of released_year and artist_count? Are there any noticeable trends or outliers?
 ![image](https://github.com/user-attachments/assets/d271dbfe-1b11-466c-ad3b-ad1146e15c50)
 ![image](https://github.com/user-attachments/assets/b681ab24-f5a7-468f-812f-661e0ea7f51f)
 
The first thing we do is declare the graphs for it to be our foundation for the graphs that we want to display in our data. we used col to display the column that we want to plot, we used binwidth for us to know the wideness of the bar in our graph, and we used df=spoti to know where we can get the data from.
As we can see from the first graph, the artist that got many streams are the solo artists. Meaning, the more artist per track, the less streams it gets. The second graph is the tracks in the released year, we can see that there are almost 800 tracks released between late 2010s and early 2020s. The third graph is the released track between 2015 to 2023. We can see that 2022 to 2023 have the highest released tracks that reached almost 600.

## Top Performers

#### Which track has the highest number of streams? Display the top 5 most streamed tracks.
![image](https://github.com/user-attachments/assets/369c1bd0-2f7d-4949-a7a9-18fc2f9eda5f)
![image](https://github.com/user-attachments/assets/531992eb-517f-4b77-a144-9f7431494e2f)

As we can see the question refers to the tracks with the highest number of streams. We used heads to get the first 5 tracks with the highest number of streams. We also used graph for us to see the different tracks and the number of streams per track. As we can see the leading is blinding lights by the weekend, the second is shape of you by ed sheeran, the third is someone like you by lewis capaldi, the fouirth is dance monkey by Tones and I, and last but not the least is the Sunflower - Spider-Man: Into the Spider-Verse	by Post Malone and Swae Lee

#### Who are the top 5 most frequent artists based on the number of tracks in the dataset?
![image](https://github.com/user-attachments/assets/27ceacb1-2668-4999-8faf-7327871b5ea9)
![image](https://github.com/user-attachments/assets/3b1fd43e-8780-40df-ba91-fe808387c055)

As we can see the question refers to the most frequent artist based on the numebr of tracks in the data set. We used heads to get the first 5 artists based on the number of tracks. We can see that the leading is taylor swift, second is the weeekend, the third one is false, the fourth is bad bunny, and the last is sza. 

#### Analyze the trends in the number of tracks released over time. Plot the number of tracks released per year.
![image](https://github.com/user-attachments/assets/5dc34a70-3c66-4f94-bedc-4cacf4ee950a)

Here, we should plot the number of tracks released per year. We declared plt.plot to plot the data and the xlabel as the year and the y label as the tracks released. We also named the graph as number of tracks released per year.
As we can see from the graph above, from 1940 to early 2010s there are less than 50 tracks released per year. However, on the late 2010s and the start of 2020, it skyrocketed to almost 400 tracks released per year.

#### Does the number of tracks released per month follow any noticeable patterns? Which month sees the most releases?
![image](https://github.com/user-attachments/assets/24c8daa9-713c-4f64-9e8c-ab5cf4d06b16)
Here, we should plot the number of tracks released per month and we used the same code as plotting the number of tracks released per year, we just replace other data since what we are looking for is years. The highest month where artist release their tracks is during april and may. The lowest track releases is during august. From may(its highest peak) the grap slowly go downward.

## Genre and Music Characteristics

#### Examine the correlation between streams and musical attributes like bpm, danceability_%, and energy_%. Which attributes seem to influence streams the most?
![image](https://github.com/user-attachments/assets/c3f3087e-01ec-4012-ac23-00618006ef14)

We can see that in the graph the song with 110 to 120 bpm has the highest streams. the song with 70 danceability has the highest streams, the songs with 50 to 55 valence has the highest streams, the song with 50 to 80 energy has the highest as well. the graph in acousticness has downtrend, the liveness has its peak at 10 and the speechiness has its peak at 5.

#### Is there a correlation between danceability_% and energy_%? How about valence_% and acousticness_%?
![image](https://github.com/user-attachments/assets/a4990d18-4fe1-45fe-b5d3-16ea4f6d7b88)
![image](https://github.com/user-attachments/assets/40b5f0f8-1a5c-4a1d-9efb-7635853c6214)


## Platform Popularity

#### How do the numbers of tracks in spotify_playlists, spotify_charts, and apple_playlists compare? Which platform seems to favor the most popular tracks?
![image](https://github.com/user-attachments/assets/456faa49-df15-41c9-b2c5-26504e846829)

We named this graph as track counts across platforms. As we can see, we compared the different numbers of tracks in spotify playlists, spotify chats, and apple playlist. I used barplot to plot the given data, as we can see the leading platform to favor the most popular tracks is in spotify playlists, the next is in apple playlists and lasly is the spotify charts.
## Advanced Analysis


#### Based on the streams data, can you identify any patterns among tracks with the same key or mode (Major vs. Minor)?
![image](https://github.com/user-attachments/assets/b9954cb9-65ab-421a-b768-569db1d07f2d)
![image](https://github.com/user-attachments/assets/4f62d2ec-0122-43bf-b0c2-477fd5e55289)

From the barplot above, there are patterns among tracks. The highest streams are the ones that uses the C# key and the lowest average streams is the one that uses G 

![image](https://github.com/user-attachments/assets/fda2c0f3-26dc-4838-ba3a-e553ee6f7a48)

From the barplot above, we can compare that the most number of average streams are the ones that uses Major mode than Minor mode. We used the barplot for us to visualize the data precisly with numbers.




#### Do certain genres or artists consistently appear in more playlists or charts? Perform an analysis to compare the most frequently appearing artists in playlists or charts.
![image](https://github.com/user-attachments/assets/7b6c14d7-800e-4baa-9675-b19c46d7423b)

I used 4 graphs to compare the artists that consistently appear in more playlists or charts. Top artist in spotify playlist, top artists in spotify charts, top artists in Apple playlist, and top artists in apple charts.
We can see that the leading artist in the spotify playlist is the weekend with over 140000 streams. The Top artist in the rest is Taylor Swift which has 500 plus in spotify charts, 1750 in Apple playlist and 1750 in apple charts.

