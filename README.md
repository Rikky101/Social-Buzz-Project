# Social-Buzz-Project
## Introduction
This project involved working with a client in the media and content industry, where our objective was to analyze user reactions to various content categories. The aim was to identify the top 5 categories based on user interactions. As part of the analytics team, I was tasked with selecting the most relevant datasets, cleaning and transforming the data, and applying necessary functions like VLOOKUP and SUMIF to derive insights. The project emphasized data modeling and category-based performance evaluation for improving client recommendations and decisions.

## Problem Statement
The key challenge was to identify the top 5 content categories based on user engagement and popularity. To achieve this, we had to analyze user reactions across different datasets, clean and prepare the data, and derive category-wise performance metrics.

## Data Sources
 Out of the 7 datasets provided by the company, I identified 3 relevant datasets for analysis:
 1. Reaction Types: This dataset contained **3 columns and 17 rows**, details about the types of reactions, Sentiment, and score.
    <https://github.com/Rikky101/Social-Buzz-Project/blob/main/reaction2.png>
 
 2. Reaction: Contained **5 columns and 25554 rows**, the reactions given by users to various content, including Content ID, user ID, types of reations, and datetime.
    
 
 4. Content: This dataset has **3 columns and 1001 rows**, captured details of the category about the content uploaded, including the content ID, content type and user ID.

## Skills Demonstrated
1. Data Transformation: Converted each dataset into table, to make it look more structured. Cleaned and prepared the datasets by removing irrelevant columns such as user ID, URL, fixing column titles, and ensuring the data was consistent.

3. VLOOKUP Function: Used to merge data from the three datasets, with the reaction datasets serving as the primary base.
   
4. SUMIF Function: Applied to calculate the total reaction scores for each category, enabling us to rank categories based on scores.

5. Find and Replace Function: Employed to ensure consistency in the Category column, replacing repeated values for accurate analysis.

6. Sorting: Sorted the data by total reaction scores to identify the top 5 most popular content categories.

**First thing! I created a copy each of the original datasets as backup for the original datasets.**

## Data Transformation
1. Reaction Dataset:
   
i. I converted the dataset to table, to make it look structured.

ii. I deleted column 1 that adds no information to the dataset, so also the UserID column

iii. Using the filter function, filtered and deleted blank rows of the type column.

iv. Formatted column title of type to Reaction_type, making it more descriptive.   

[Reactions.csv](https://github.com/user-attachments/files/17717751/Reactions.csv)


3. Content Dataset: In this dataset, I deleted the URL and User ID columns to reduce unnecessary information. I also changed the column title from "Category" to "Content Category" and "type" to "Content Type" for clarity. To ensure consistency, I used the Find and Replace function to eliminate repeated values in the Category column.[Content.csv](https://github.com/user-attachments/files/17716960/Content.csv) 


4. Reaction Types dataset: This dataset was cleaned and prepared for analysis without requiring further modifications. [ReactionTypes.csv](https://github.com/user-attachments/files/17716948/ReactionTypes.csv)

## Analysis and Visualization
The analysis aimed to identify the top 5 content categories based on user engagement by integrating data from the Reaction, Reaction Types, and Content datasets. Key functions such as VLOOKUP and SUMIF were employed to merge the datasets and calculate reaction scores.

Visualizations, including bar charts, were used to showcase the top 5 content categories, reaction types, and the content type with the highest user engagement, providing valuable insights for Social Buzz. Additionally, slicers and timelines were added using the sentiment and datetime columns, respectively, to enhance data interactivity.[Social Buzz Project.xlsx](https://github.com/user-attachments/files/17717611/Social.Buzz.Project.xlsx)


## Conclusion and Recommendtaion
 The analysis revealed that animal content received the highest user engagement with 1,897 reactions, while audio content had the lowest engagement. Furthermore, the heart reaction was identified as the most frequently used reaction type.
Recommendations include:
 1. Continue prioritizing content in the top-performing category (Animal Content)
 2. Given that the heart reaction was the most commonly used, future content could be designed to elicit positive emotional responses from users, increasing overall engagement.
 3. The "Scared" reaction was predominantly associated with negative responses. Social Buzz should consider minimizing content that may trigger this reaction to avoid negatively impacting user sentiment.
 4.  Regularly track engagement metrics over time to identify emerging trends and adjust the content strategy accordingly.



