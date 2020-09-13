# David House Homework 1 due 9/17/2020

## How to Navigate this Project

---

This project contains two folders each with a single file. The `Data` folder contains a .json file which was retrieved from [here](https://json.reddit.com/r/pics/top/?limit=100). This represents the top 100 posts of all time on the r/pics subreddit. The `Code` folder contains a jupyter notebook which I used to clean and analyse the data.

## My goals for this project

---

I was interested in looking at data taken from the web for my project. To do this I used the popular social media site www.reddit.com. This site allows users to upload pictures links and other media for other users to comment on and share. A unique feature of reddit is that users are able to upvote and downvote posts causing posts with more votes to move to the top where more people can see them. I wanted to see if there was any effect on the length of a posts title and how popular it became. 

## Obstacles during my project

---

* Using urls to access the reddit API I was unable to get more than the top 100 posts to a given subreddit. I think that had I been able to get all posts ever created for r/pics I would have a better idea of the effect that tile length has on a posts popularity. 


## Methods

---

1) My first step was to obtain usable data which I got from the subreddit r/pics. I used the reddit API to get a .json representation of the top 100 posts on r/pics

2) Once I had the data I used pandas to dig into the data. Since I was intersted in the titles of each posts I used a combination of lists, for loops and dictionaries to get the titles into a usable data structure.

3) My result from the previous step gave me a dictionary in the form `{"Title": number of words in title}` which I then converted into a `DataFrame`

4) Using the `DataFrame` I sorted the data using `sort_values()` then I described the data using `describe()` finally I plotted the data in a histogram.

## Results

---

|  | Word Count|
| :-------------: | :-----------: |
|count        |100|
|mean         | 16.090000|
|std           |10.524714|
|min            |2.000000|
|25%           | 9.750000|
|50%           |14.500000|
|75%           |20.250000|
|max           |51.000000|

**Scatterplot comparing popularity of post to length of title**

![Image](https://github.com/DavidBrynnHouse/Data_601_HW-1/blob/master/Images/ScatterPlot.png)


**Box plot highlighting several outliers**

![Image](https://github.com/DavidBrynnHouse/Data_601_HW-1/blob/master/Images/Box-Plot.png)

## Conclusions

---

Becuase I only have the top 100 posts from r/pics I hesitate to draw many conclusions without a loss of generality. However I can see that most posts have fewer than 20 words. This may change depending on the subreddit since mods are able to specify a minimum and a maximum title length[3]

## Bibliography

---

[1]www.reddit.com

[2]https://json.reddit.com/r/pics/top/?limit=100

[3]https://mods.reddithelp.com/hc/en-us/articles/360010322091-Post-Requirements

