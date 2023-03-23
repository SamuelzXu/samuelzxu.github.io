--
layout: post
title: NASA Cyanobacteria Challenge
--

# Introduction

## Background 

I participated in a data science competiton ending on Febrary 17, and was fortunate to score in the top 3%. This is a post on my approach and challenges I encountered.

First, a little background on the topic is in order. [Cyanobacteria are](https://www2.gnb.ca/content/gnb/en/corporate/promo/cyanobacteria.html) microscopic bacteria found in bodies of water which feed off of sunlight. Although the term algae is mostly reserved for eukaryotes, cyanobacteria are still oftentimes referred to as "algae". They are omnipresent in most fair climates, but as with most things, the extremes are troublesome for humans. When conditions allow, cyanobacteria will reproduce at incredible rates. Certain kinds of cyanobacteria [release harmful toxins](https://www.epa.gov/cyanohabs/health-effects-cyanotoxins) as waste byproduct, and when their abundance is extraordinary, the result is a [Harmful Algal Bloom](https://www.noaa.gov/what-is-harmful-algal-bloom) (HAB) that poisons the water sources they are present in. 

## The Goal

The goal of this challenge is to detect and identify the severity of algal blooms in water bodies across the continental United States (CONUS).

For data, we were permitted access to the following:
- Satellite imagery spanning 2013-present, specifically [Landsat](https://planetarycomputer.microsoft.com/dataset/group/landsat) and [Sentinel](https://planetarycomputer.microsoft.com/dataset/sentinel-2-l2a)
- Climate data from the [High Resolution Rapid Refresh](https://rapidrefresh.noaa.gov/hrrr/) (HRRR) index
- Digital Elevation Model (DEM) data from [Copernicus Satellite](https://planetarycomputer.microsoft.com/dataset/group/copernicus-dem)

# My Approach

First, I recognized that this was a highly complicated set of data that I was unfamilar with, and I needed a way to organize and visualize the tasks, ideas, and research topics I planned to execute on. Initially, I played around with a [developer instance of JIRA](https://developer.atlassian.com/platform/marketplace/getting-started/), but I decided that it was too specialized for working in teams - I was only working by myself, and most features of JIRA would incur unnecessary overhead. I settled on Google Sheets for this, and laid out a basic framework tracking my ideas. At the beginning of the challenge, it looked like this:

![EmptyVizualizer]({{ site.baseurl }}/images/empty-viz.jpg)

I eventually adopted a coloring scheme to signify progress, used strikethroughs to signify failed ideas, and filled the table out nicely. By the end of the challenge, it looked like this:

![Vizualizer]({{ site.baseurl }}/images/viz.jpg)

As you can see, every approach, idea, research direction, question, and feature had to be approached systematically. Otherwise, this would have been a true headache to keep track of. Initially I knew very little about cyanobacteria and factors influencing their abundance, and even less about method of accessing satellite and climate data, so the task at hand seemed daunting.

