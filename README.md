# dbt™ Data Modeling Challenge - Social Media Edition

## Project Title: Having an Impressive Youtube Channel

Welcome to the [dbt™ Data Modeling Challenge - Social Media Edition](https://www.paradime.io/dbt-data-modeling-challenge)! This challenge invites you to showcase your data modeling skills using social media data.

## 📋 Table of Contents

1. [Introduction](#introduction)
2. [Data Sources](#data-sources)
3. [Methodology](#methodology)
4. [Insights](#insights)
5. [Conclusions](#conclusions)

## Introduction

- How do people get upto 1M views on their youtube channels?

- How can I have a youtube channel that could fetch thousands of dollars?

- Why is my youtube channel subscribers not running into hundreds of thousands of subscribers?

If you've had questions like these on your mind, then we might be on the same page? Whether you're thinking of having a youtube channel or already have a youtube channel that's stuck on low views, low subscribers and low engagement in general, this analysis could change your perspective about the usual youtube channel and move you to having an unusual youtube channel (one with millions of engagements). So how about we dig in and get into the analysis right away...

## Data Sources

My analysis was based on data sources from Paradime and other sources.

The Paradime data source includes the hackernews data provided in the competition.

Additional Data Sources:

- [Youtube Data API](https://developers.google.com/youtube/v3) where data metrics from different youtube channels across different countries were extracted. Thanks to [@Mithelljy](https://github.com/mitchelljy) for his [Trending Youtube Scraper Python Script](https://github.com/mitchelljy/Trending-YouTube-Scraper/blob/master/scraper.py)

- [Google Trends Data](https://trends.google.com/trends/)

- [Python Reddit API Wrapper](https://praw.readthedocs.io/en/stable/) where reddit data was extracted using my python script. This python script also did some sentiment analysis on the comments and posts extracted based on my specific keyword.

## Methodology

### Tools Used:

- [Paradime](https://www.paradime.io/) for SQL, dbt modeling

- [Hex](https://hex.tech/) for data visualization

- [Motherduck](https://motherduck.com/) for data storage

- Python for data extraction and sentiment analysis

- Microsoft Excel to transform data gotten from Google Trends before moving them into Motherduck

### Data Preparation Techniques

- Selected distinct values in various data sources pulled into Motherduck to prevent duplicate values

- Use of dbt tests to test for uniqueness and desired relationships between tables

- Ensured structured header layout of csv files gotten from Google Trends

- Merged the different countries youtube data extracted from the Youtube data api into one table using dbt while using a 'country' flag column to distinguish the data coming from different countries

- Carried out sentiment analysis on reddit posts and comments using python

- converted columns into their respective data types to aid analysis

## Insights