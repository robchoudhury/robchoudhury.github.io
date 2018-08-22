---
title: Miami Mango Ratings
author: Robin Choudhury
date: '2018-08-22'
slug: miami-mango-ratings
categories: []
tags: ["data science", "agriculture", "random"]
header:
  caption: 'Outrun Mangos: had a blast in Miami, thought the Outrun style was awesome'
  image: 'img_mango/20170714_063234-min.png'
---


Mangos are grown widely in South Florida, but only a few varieties ever make it north, because they don’t really ship well and there isn’t a huge market. I ended up receiving some rare varieties from a collaborator down south, and I wanted to know how they ranked one to another, so my wife and I rated the different varieties.

## The Data

My wife and I rated the mangoes over the course of about a week, tasting the different varieties as they felt more and more ripe. We each did a subjective rating of 1-10, with 1 being "this tastes terrible", and 10 being "this is literally the best mango I've ever had". We rated independent of each other, recording our ratings, and I collated the data for this dataset.

## How Did They Perform?

![]("img_mango/variety_rating.png")

So overall, it looks like *Kensington Pride*, *Hayden*, and *Edwards* were clear winners, and the other varieties were not. What happened?

If you look at the other data in the file (filled with NA's, sorry) there are notes on the stringiness and the taste of the varieties. Poor varieties like *Sweet Tart* had chalky texture in the mouth, and would sometimes smell like tylenol, or have no aroma at all. Good performers had very slight to no stringiness, and had the kind of 'quintessential' tastes of mango: fruity, tropical, rich. *Kensington Pride* was my favorite, and it tasted a bit like muscadine grapes. Mid-performers like *Nam Duk Moi* had stringiness, and *Dot* would sometimes have a popcorn like flavor, or tasted too sweet.

Did my wife and I have different views on these mangos?

![]("img_mango/person_rating_dumbbell.png")

We had fairly similar ratings, but it looks like I pretty consistently rated things more favorably than she did.

## Conclusions

If you are in Miami area in July, you NEED to taste mangoes. They grow on street trees, make friends, knock on doors, see if people will sell them to you. Have fun!
