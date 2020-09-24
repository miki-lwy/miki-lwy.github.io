---
layout: page
title: Portfolio
date: Sun Apr 26 09:49:43 2020
categories: private
permalink: /portfolio/
---
# Spotify's Music Analysis - 17 October 2018
#### This is my first school project in Hyper Island

You can find the source code at GitHub:
[Spotify](https://github.com/miki-lwy/spotify)
and the original presentation [HERE](https://drive.google.com/file/d/1cgluz0P8YpWzI08buF6mijGV1Jqswv95/view?usp=sharing)


This project is going to answer the following questions:

1. Similar music taste among different countries

2. Which country has the most similar taste with the global music?

3. Does HK anti-extradition protest affect the users from HK listening to more upset songs?

#### **LIBRARIES USED**
- Spotify Web API
- Fycharts
- Pandas
- Matplotlib
- Seaborn

#### **LIMITATION**

- Spotify Web API does not provide top songs for each region/ country

- Spotify chart is the only alternative

- Spotify chart only provides information:

    1. Top 200 daily/ weekly

    2. Top 50 viral daily/ weekly

- Dataset is small

#### **ASSUMPTION**

Top 200 Daily’s dataset is not significantly different from Top 200 weekly’s

#### **DATASET**
Period: 2018-09-21 - 2019-09-27

Data Interval: Weekly basis

Number of Countries: 63 + Global

**PART I - SIMILAR MUSIC TASTE AMONG DIFFERENT COUNTRIES**

#### **OPERATIONAL DEFINITION**

How do we know if one country shares a music taste with another?
Then, an operational definition comes into play!

Jaccard similarity fits the best for such analysis.

![Jaccard Similarity](/assets/images/Jaccard Similarity.jpg)

![ClusterMap: Music Similarity among different countries](/assets/images/Music Similarity among different countries.png)

From the above clustermap, there were several clusters representing their own specific music tastes.
The spanish-speaking countries shared the same music taste, so did Asia and German-speaking countries. However, France and Italy had their specific music taste and so did Brazil and Turkey. They shared nothing in common with other countries in music context. 

In conclusion, music taste seemed to have something to do with the shared languages and geographical distance.

**PART II - WHICH COUNTRY HAS THE MOST SIMILAR TASTE WITH THE GLOBAL MUSIC**

## Which Country has the most similar music taste with Global 200?
![HeatMap: Similar Music Taste with Global 200](/assets/images/Similar Music Taste with Global 200.png)

**PART III - DOES HK ANTI-EXTRADITION PROTEST AFFECT THE USERS FROM HK LISTENING TO MORE UPSET SONGS?**

#### **OPERATIONAL DEFINITION**
How do we know whether a song is happy or not?

Thanks for the audio features - Valence provided by Spotify API, we can measure it!
![Audio feature - Valence](/assets/images/audio feature.png)

## Music Valence Over Time - Hong Kong
![Audio feature - Valence HK](/assets/images/Music Valence HK.png)

Well... As you can see from the above graph, the valence fluctuated around 0.4 - 0.45. I couldn't conclude that the users in HK listening to more upset song was due to HK anti-extradiction protest. 

Hmm...Let me think! Is it because the life in Hong Kong is always difficult. We have crazy housing price in the world. We don't have job security like minimum wage implemented. What about reversing our thinking to look at those happy countries? Do the users in the happiest countries listen to more happy songs?

First, we need to identify which are the top happiest countries in the world. 


**PART III-2 - DO HAPPIEST COUNTRIES LISTEN TO MORE HAPPY SONGS?**

## Happiest countries in the world - 2019 ranking
![Happiest countries in the world - 2019 ranking](/assets/images/Happiest countries in the world 2019 ranking.png)

So, I run the same methodology but with the happiest countries this time.
And we got the below result:
## Music valence over time - Switzerland
![Audio feature - Valence Swiss](/assets/images/Music Valence Swiss.png)

Well...It fluctuated around 0.45 - 0.5 this time. It's a bit flat. I failed to make the conclusion that happiest countries listened to more happy songs :(


## Can I make a conclusion?
**X Does HK anti-extradition protest affect the users from HK listening to more upset songs?**

**X Do happiest countries listen to more happy songs?**



Hmm...So, what are the factors driving behind?
Let's go back to my original question.

Does HK anti-Extradition protest affect the users from HK listening to more upset songs?

HK anti-extradition protest started from June to now (3 months only). Usually, it takes time to reflect something on the data. What if something happens more regularly? For example, regular events like Christmas and Summer holidays. Will we get different result?
Let's make another hypothesis!

So, I run the same methodology but with all the countries this time.
And we got the below result:
**PART III - DO PEOPLE LISTEN TO MORE HAPPY SONGS DURING HAPPY HOLIDAYS?**

## Music valence over time across different countries
![Audio feature - Different Countries](/assets/images/Music Valence Across Different Countries.png)

The darker the color, the happier the song the users listened to.
As for Germany, the users seemed to listen to more happy songs around mid-December (X'Mas) and also from July to August (Summer time). We also observed similar pattern for Belgium, Singapore, the USA and Argentina.

Let's see one more example - Indonesia.

## ONE MORE EXAMPLE ...
![Audio feature - Indonesia](/assets/images/Music Valence Indonesia.png)

Why couldn't we find the similar pattern as before? Moreover, it exhibited a different pattern. The first half is darker than the second half. But if we are aware of the location of Indonesia. It's actually situated in the equator. That means when we have winter, they have summer. When we have summer, they have winter. That explained what could happen here!


Thank you for your reading :)

I hope you will find it interesting.

