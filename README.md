# imdb_movie_analysis_project

## Table of Contents

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Data Cleaning](#Data-Cleaning)


## Project Overview
---
This project aims to help a film production company develop a successful movie by analyzing IMDB movie data. The analysis will examine various factors contributing to film success.


## Data Sources

IMDB Movie Data: The primary dataset used for this analysis is the "IMDB Movie ANALYSIS.xlsx" file, containing detailed information about various movies. 

## Key Performance Indicator (KPI)
- Success Definition: A film is considered successful if its profit is greater than its budget.

## Direct KPIs
- Director Name: Analyzing the directors of successful films to identify any commonalities or notable patterns.
- Actor Name: Studying the actors in successful films to understand their impact on a film's success.

## Data Cleaning 

#### 1. Remove irrelevant columns from data set 
plot_keywords
- contain a set of keywords related to important themes or elements in the film. These keywords help in identifying key aspects of the film's plot.

#### 2. Remove Special Characters 
- In the dataset, I removed the character "Â" from all movie titles. This character appeared in titles

![image](https://github.com/user-attachments/assets/add8a70e-1a3b-4ab6-839d-7f2dba0a9099)

#### 3. Handling missing values
- Replaced blank values in the "language" column with "English".
  - Before
  
![image](https://github.com/user-attachments/assets/0d07b0be-538b-470b-9487-742be43534d2)
  - After

![image](https://github.com/user-attachments/assets/63a443b6-45c6-446f-a59f-c73d90968eb4)

 #### 4. Creation of "Success or Failure" Column
- Action: Added a calculated column named "Success or Failure".
- Formula: =IF([@gross] > [@budget], "Success", "Failure")
- Purpose: This column was created to categorize films based on their financial performance. If a film's gross revenue is greater than its budget, it is labeled as "Success"; otherwise, it is labeled as "Failure".

![image](https://github.com/user-attachments/assets/ac0fe1b1-2370-42b2-8a1d-dea921a9d781)

## Data Analysis
To identify patterns and factors contributing to the success of films, I created three pivot tables to analyze the data from different perspectives:
Success or Failure	Success
![image](https://github.com/user-attachments/assets/5dbbcdef-aada-4685-baf0-7db07e8971e8)

### Best Directors
- Purpose: To identify the directors associated with the most successful films (where profit > budget).
### Best Actors
- Purpose: To determine the actors who frequently appear in successful films.
### Best Actors and Directors
- Purpose: To examine the combination of actors and directors that leads to the highest film success rates.

