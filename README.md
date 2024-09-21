Overview
========
Data engineering pipleine for storing, analyzing and visualizing stock market behavior based on a variety of factors.

Focus Areas
===========

- **Data Acquisition**
  - Where is the data coming from? (API, database, file systems, documents)
    - In our case we have a single datasource of history stock data in text files that need to be parsed in the next phase.
    - If we need more modern data, we can pull from free datasets (just requires registration) from https://paperswithbacktest.com/ on HuggingFace .
      - https://huggingface.co/paperswithbacktest
    - Included in these datasets are historical news which will be a nice source of events for relational analysis
    - It is possible that we will write a Twitter scrapper to scrape the tweets of CEOs and C-Suite executives if we want to see what happens when they act a certain way (does it affect stock prices?)
    - House and Senate Financial Records / Disclosures      
- **Data Cleaning / Formatting**
  - When pulling from datasets that are already cleaned, you don't have to do much here but in the real world, data is messy.
  - When data comes from various sources, you might need to "normalize" the data before you store it. We will get some practice with this since we will be pulling from 3 or 4 sources.
  - Python scripts will be created for this task.  
- **Data Storage**
  - We need to pick a database / data storage solution.
  - Find the solutions that have a free Tier but are also in demand by top companies that are hiring data engineers. 
- **Data Analysis**
  - The fun part! Analyze the data!
  - What are we trying to solve/prove/observe/demonstrate/study?
    - Idea #1: Does the personal life or social media posts of CEOs have a direct affect on stock prices of their companies?
    - Idea #2: What's the trading track record of members of Congress/Senate?
      - We could take this further an analyze if any of their activities in government would have influenced the prices of those comapanies (regulations **_do_** impact stock prices!).
    - Idea #3: Do predictable events (fed rates, mortgage rate, the opening/closing of markets, etc.) have any affect on stock price?
    - Idea #4: What kind of news or event is required to move a stock price?
    - Idea #5: ...
    - Each analysis option gives us a chance to use different techniques or strategies as a learning opprotunity. This is where 80% of the logic (and blood, sweat, and tears) will live. 
- **Data Visualization**
  - Visualize everything with interactive capabilities.
  - The goal is to make the data "pretty" and to let it tell a visual story
  - We will use Streamlit for the interface
---
