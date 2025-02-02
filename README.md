## Audio Reccomendation Algorithm

This is an unsupervised learning task that aims to come up with an algorithm that is able to do audio reccomendations from a data set. This project utilizes dataset of songs from 1950 to 2011, it contains a mix of lyrical and continuous variables pulled from a 2020 research: https://data.mendeley.com/datasets/3t9vbwxgr5/3

## Report

The EDA had a wealth of insightful information. It can be stated that the data set contained an unequal distribution of genres, with Pop being the most prevalent and Hip Hop the least. Some genres had dominating emotion scores, such country music, which had a predominant sadness score. An other intriguing observation was the shift in some Emotion ratings over the years; romantic feelings saw a decline in ratings as the decades went by, while scores for violent emotions increased.
![alt text](/images/VSOT.png) ![alt text](/images/RSOT.png)

Other than the fact that Age and Release Date have a perfect negative connection and that Obscene Score and Song Length have a positive correlation of 0.44, there weren't many correlations between the variables. Furthermore, there is a marginally stronger negative association (-0.27) between the Sadness score and the Obscene score.
![alt text](/images/CH.png)

I was able to determine through EDA that most of the columns would have to be retained because they provided a variety of insightful data regarding the characterization and grouping of the songs. Since the lyrics and track names were idiosyncratic and didn't provide any information for the EDA or help group the music, I dropped them.


Once the data was set for modeling I first utilized the Elbow Method to identify the best number of clusters. Even though the elbow of the graph is estimates the optimum number of clusters as 2, I decided to got a bit over the elbow at 3 in order to maintain a more complex clustering .


Particular genres and the prevalence of particular Emotion Ratings were detected by the system. For instance, cluster 2 has a large number of songs about dating and sadness. It also detected songs from other countries and genres, possibly as a result of the varying emotions that songs conveyed in various contexts within the same decades.

The cluster pertains to broader suggestions based on the Emotion Ratings. For example, if I had to suggest a song to the user, I would pay closer attention to the rows with genres like rock, blues, pop, country, and reggae that are more in line with their existing musical tastes. Such as "Necessary Evil" by Frankie Laine and other songs included in the recommendations table.