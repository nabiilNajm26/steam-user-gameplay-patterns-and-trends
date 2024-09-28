
# Analysis of Steam User Gameplay Trends and Patterns

## Project Background
In the digital age, game distribution platforms like Steam have become a rich source of data on user behavior and preferences. With over 100 million user reviews, this data provides valuable insights into trends and patterns in user gameplay that can be leveraged by game developers, marketers, and researchers. This project aims to analyze the trends and patterns of Steam users' gameplay, focusing on various aspects such as playtime, game popularity, and gameplay behavior based on time and region.

## Problem Statement
This project aims to answer several key questions:
- How do user gameplay patterns change over time (e.g., weekends vs. weekdays)?
- What games are the most popular in different regions?
- How much time do users spend playing certain games?

By answering these questions, this project will provide insights that can be used to optimize marketing strategies, game development, and user experience enhancement.

## Dataset
- **Source:** Steam user reviews dataset
- **Size:** 17 GB (compressed), 43.19 GB (extracted)
- **Columns:** 24 columns including `recommendationid`, `appid`, `game`, `author_steamid`, `author_playtime_forever`, `author_playtime_last_two_weeks`, `timestamp_created`, etc.

## Tools and Technologies
- **Docker**: For container management
- **Python**: Main programming language
- **Polars**: For data processing and transformation
- **Apache Airflow**: For managing the batch processing pipeline
- **PostgreSQL/MySQL**: For storing processed and analyzed data
- **Grafana/Metabase**: For visualizing the analysis results in interactive dashboards
