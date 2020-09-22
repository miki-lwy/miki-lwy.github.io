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
![Jaccard Similarity](/assets/images/Jaccard Similarity.jpg)

![ClusterMap: Music Similarity among different countries](/assets/images/Music Similarity among different countries.png)


**PART II - WHICH COUNTRY HAS THE MOST SIMILAR TASTE WITH THE GLOBAL MUSIC**

## Which Country has the most similar music taste with Global 200?
![HeatMap: Similar Music Taste with Global 200](/assets/images/Similar Music Taste with Global 200.png)

**PART III - DOES HK ANTI-EXTRADITION PROTEST AFFECT THE USERS FROM HK LISTENING TO MORE UPSET SONGS?**

#### **OPERATIONAL DEFINITION**
![Audio feature - Valence](/assets/images/audio feature.png)

## Music Valence Over Time - Hong Kong
![Audio feature - Valence HK](/assets/images/Music Valence HK.png)

**PART III-2 - DO HAPPIEST COUNTRIES LISTEN TO MORE HAPPY SONGS?**

## Happiest countries in the world - 2019 ranking
![Happiest countries in the world - 2019 ranking](/assets/images/Happiest countries in the world 2019 ranking.png)

## Music valence over time - Switzerland
![Audio feature - Valence Swiss](/assets/images/Music Valence Swiss.png)

## Can I make a conclusion?
X Does HK anti-extradition protest affect the users from HK listening to more upset songs?

X Do happiest countries listen to more happy songs?

**PART III - DO PEOPLE LISTEN TO MORE HAPPY SONGS DURING HAPPY HOLIDAYS?**

## Music valence over time across different countries
![Audio feature - Different Countries](/assets/images/Music Valence Across Different Countries.png)

## ONE MORE EXAMPLE ...
![Audio feature - Indonesia](/assets/images/Music Valence Indonesia.png)

Thank you for your reading :)

I hope you will find it interesting.

