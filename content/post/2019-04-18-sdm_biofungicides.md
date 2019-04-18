---
title: Spinach Downy Mildew Biofungicide Trials
author: Robin Choudhury
date: '2019-04-18'
slug: sdm-biofungicides
categories: []
tags: ["data science", "biology", "random", "agriculture", "mycology"]
header:
  caption: 'Steve Koike applying some biofungicides in a trial in the Pajaro Valley.'
  image: 'img_sdm/IMG_1050.JPG'
---

Full analysis is [here](https://github.com/robchoudhury/sdm_biofungicide)

Published in Plant Disease Management Reports [2014](https://www.plantmanagementnetwork.org/pub/trial/pdmr/volume9/abstracts/v22.asp), [2015](https://www.plantmanagementnetwork.org/pub/trial/pdmr/volume10/abstracts/v016.asp), and [2016](https://www.plantmanagementnetwork.org/pub/trial/pdmr/volume11/abstracts/v017.asp).

Throughout my PhD work, it became obvious that the challenges of spinach downy mildew were most heavily impacting organic growers. They were unable to rely on conventional synthetic pesticides that were able to suitably control disease in the conventional crop, and had to rely on resistance to control the disease. I wanted to see if any biofungicide had effect on the disease. I am using the term 'biofungicide' broadly here, meaning any form of pesticide that would be organically based. So this could be things derived from microbes (like Serenade), things derived from naturally occurring chemicals (like Copper), or any organism that would directly impact or prevent disease. We ended up running eight trials over the course of three years, and four of them ended up with disease. Each trial had an untreated control and used a conventional (synthetic) control chemical. I sprayed 2-4 times over the course of 4 weeks, and rated for disease incidence in plots.

# The Results

![](/img/img_sdm/fungicidecairo.png)

When we look across all of the chemicals that were used, we see that none of them were able to completely prevent disease, although some were able to significantly reduce disease compared with the untreated control. This suggests that they may be useful in helping to prevent disease in combination with other control options. Trial #2 got a bit out of hand with a late application due to unforseen rain delays, resulting in very high disease ratings, even for the standard chemical control.

# Normalizing the Results

But not all of the chemicals were tried in all of the trials. Some became unavailable in later trials, others were introduced to us or growers asked us to trial, and space limitation made it difficult for a few trials. One way to account for this is through meta analysis, although four trials is not nearly enough to do a proper meta-analysis. One alternative is simply to normalize each disease incidence rating to the mean of the untreated control for the trial. This had the result of scaling disease from 0 (complete control compared with untreated control) to infinity (much, much worse than the untreated control), although most of the products fell between 0 and 1. Some of the products (e.g. Actigard, Biospecific, Lifegard, Howler, Zonix) were only included in one trial that ended up with relatively low disease, so they are kind of artifically lower in disease incidence than other products.

![](/img/img_sdm/fungicidecairo_colored_sorted_scaled.png)

# Conclusions

These results suggest there are potential control measures for disease, although they don't seem to completely remove disease risk.