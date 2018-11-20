---
title: Homestead Avocado Ratings
author: Robin Choudhury
date: '2018-11-20'
slug: avocado-ratings
categories: []
tags: ["data science", "agriculture", "random"]
header:
  caption: 'Avocado hunting: the wild and elusive Dr. Jonathan Crane (UF-TREC) harvesting some avocados'
  image: 'img_lw/IMG_20181003_173924.jpg'
---

[Full analysis here](https://github.com/robchoudhury/avocado_tasting)

Global avocado production mostly focuses in Mexico, with the most prominent variety being 'Hass'. I work on a project researching a disease of avocados (and other plants in the same family, Lauraceae) that causes rapid death, laurel wilt. Avocados in Florida are threatened by laurel wilt. Most production occurs in Miami-Dade county, mostly around the Homestead production region. The avocados grown in Florida tend to be of the West Indian races, whereas Hass are Mexican-Guatamalan hybrid races. West Indian races are larger (think about the size of a grapefruit) and are more watery and floral than Hass. Most of the varieties grown in south Florida are not exported because they don't ship well. I was fortunately to go down and gather some avocados from the University of Florida Tropical Research and Extension Center (UF-TREC), where my collaborator [Dr. Jonathan Crane](https://trec.ifas.ufl.edu/faculty/jcrane/) works. I brought them back north to the [Garrett lab in Gainesville](http://www.garrettlab.com/), where we tasted and rated the avocados as they became ripe. 

Here they are!
![](/img/img_lw/IMG_20181008_084604.jpg)


## The Data

We rated the avocados over the course of about a week, and I have to be honest, by the end I didn't want to see another avocado again for a long time. Eating one avocado is a joy; eating 10 in a very short time span is a slog. In addition, not all of them were very good! Some were better than others, but most of the reviewers thought that the Hass was probably better than most of these. That said, our palates (palletes? I'm still thinking about [the last blog post](https://robchoudhury.netlify.com/post/colors/)) have been refined to enjoy Hass. If we had grown up with these varieties, we might have had more positive thoughts on them. It took about a week for all of the fruit to ripen, and we ate them as they became ready.  We each did a subjective rating of 1-10, with 1 being "this tastes terrible", and 10 being "this is literally the best avocado I've ever had / this is as good as Hass". We rated independent of each other, recording our ratings, and I collated the data for this dataset. Not everyone rated all avocados (except for me), but most people rated at least two.

## How Did They Perform?

![](/img/img_lw/2018-11-20.variety.rating.png)

So overall, it looks like *Lara Red*, *Tonnage*, and *Pahokee* were top of the heap, but the others were all close behind.

Most of the avocados were rich, but not quite as rich as a typical *Hass*, which has a nice butteryness and clean mouthfeel. Some of the avocados were watery, which definitely cost them points. Others had distinct off-flavors, kind of vegetative or acrid. 

## Did people have different views on the avocados?

![](/img/img_lw/2018-11-20.variety.rating.person.png)

YES! Overall, some people were quite positive about some varieties and negative about others. However, most people had similar ratings across the board, with only a few people with distinct opinions on the avocados. Kelsey and I rated the most avocados over the period, so ours tended to be the most negative. I was curious if there was a relationship between the number of avocados that we rated and the mean avocado rating we had, so I did a simple linear regression of the two. 

![](/img/img_lw/2018-11-20.variety.rating.lm.png)

There was a decent relationship between the two, with an R^2 of 0.4447 and a p value of 0.0297. It seems that for every additional avocado a person rated, their mean rating score dropped by about 0.2, which is noticable. 

## Was there an effect of time?  

![](/img/img_lw/2018-11-20.variety.rating.date.png)

YES! It looks like as the week wore on, people got more and more tired of avocados. While the first few varieties garnered wide support, the later varieties were not as popular. However, its difficult to disentangle the effect of rating date with variety itself, as we did not taste the varieties all on the same day, but rather on sequential days. 

## Did Raters Group Together?

![](/img/img_lw/2018-11-20.variety.ordination.png)

I have been looking into community analyses, and I wanted to know whether the ratings performed by each person could help to group the raters into 'camps'. I used the 'decorana' function within the 'vegan' package to conduct a detrended correspondance analysis. I had to fill in the gaps for how people rated, and I filled them in with zeros, which probably screwed up the data and analysis somewhat. It looks like Ricardo and I rated things similarly, and Kelsey and Yanru rated their similarly, but overall there was quite a bit of differentiation among raters.

## Conclusions

If you are in the Miami or Homestead area, try to get your hands on some of the local varieties. They weren't all winners, but it was really interesting to taste the West Indian types and see how they all compare with one another.
