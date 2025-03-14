# Social-Buzz-Project
## Introduction
This project involved working with a client in the media and content industry, where our objective was to analyze user reactions to various content categories. The aim was to identify the top 5 categories based on user interactions. As part of the analytics team, I was tasked with selecting the most relevant datasets, cleaning and transforming the data, and applying necessary functions like VLOOKUP and SUMIF to derive insights. The project emphasized data modeling and category-based performance evaluation for improving client recommendations and decisions.

## Problem Statement
The key challenge was to identify the top 5 content categories based on user engagement and popularity. To achieve this, we had to analyze user reactions across different datasets, clean and prepare the data, and derive category-wise performance metrics.

## Data Sources
 Out of the 7 datasets provided by the company, I identified 3 relevant datasets for analysis:
 1. Reaction Types: This dataset contained **3 columns and 17 rows**, details about the types of reactions, Sentiment, and score. [ReactionTypes.csv](https://github.com/Rikky101/Social-Buzz-Project/blob/main/ReactionTypes%20(1).csv)
 2. Reaction: Contained **5 columns and 25554 rows**, the reactions given by users to various content, including Content ID, user ID, types of reations, and datetime.[Reactions.csv](https://github.com/Rikky101/Social-Buzz-Project/blob/main/Reactions.csv)
 3. Content: This dataset has **3 columns and 1001 rows**, captured details of the category about the content uploaded, including the content ID, content type and user ID. [Content.csv](https://github.com/Rikky101/Social-Buzz-Project/blob/main/Content.csv)

## Skills Demonstrated
1. Data Transformation: Converted each dataset into table, to make it look more structured. Cleaned and prepared the datasets by removing irrelevant columns such as user ID, URL, fixing column titles, and ensuring the data was consistent.

3. VLOOKUP Function: Used to merge data from the three datasets, with the reaction datasets serving as the primary base.
   
4. SUMIF Function: Applied to calculate the total reaction scores for each category, enabling us to rank categories based on scores.

5. Find and Replace Function: Employed to ensure consistency in the "Category" column, replacing repeated values for accurate analysis.

6. Sorting: Sorted the data by total reaction scores to identify the top 5 most popular content categories.

**First thing! I created a copy each of the original datasets as backup.**

## Data Transformation
1. Reaction Dataset:
   
   i. Converted the dataset to table, to make it look structured.
   
   ii. Deleted "column 1" that adds no information to the dataset, so also the "UserID column".
   
   iii. Using the filter function, filtered and deleted blank rows of the "type" column.
   
   iv. Formatted column title of type to "Reaction type", making it more descriptive.
     
    v. Used the **text** function to fornat the datetime column into date and time redpectively.
   
Voila! The reaction dataset is cleaned and ready for analysis. [Reaction_Dataset](https://github.com/Rikky101/Social-Buzz-Project/blob/main/Reactions_cleaned.xlsx)

2. Content Dataset:
   
   i. Converted the dataset to table, to make it look structured.
   
   ii. Deleted "column 1" that adds no information to the dataset, so also the "UserID" and "URL" column.
   
   iii. Formatted "Type" and "category" to "Content type" and "Content category" respectively.
   
   iv. There were inconsistencies in the "Content category", using the **Find & Replace function**, it was corrected to give the dataset 
       a clean and final look.
   
   Ready for analysis! [Content_Dataset](https://github.com/Rikky101/Social-Buzz-Project/blob/main/Content_cleaned.xlsx)

4. Reaction Types dataset:
   
   i. Converted the dataset to table, to make it look structured.
   
   ii. Deleted "column 1" that adds no information to the dataset.

   iii. To make the field consistent, "type" column was formatted into "Reaction type"

Ready for analysis! [Reactiontype_Datatset](https://github.com/Rikky101/Social-Buzz-Project/blob/main/ReactionTypes_cleaned.xlsx)
  
## Analysis and Visualization
The three cleaned datasets were merged into a single comprehensive dataset for analysis and visualization, with **Vlook up function**. [Final_Dataset](https://github.com/Rikky101/Social-Buzz-Project/blob/main/Final%20dataset.xlsx)

Visualizations, including bar charts, were used to showcase the top 5 content categories, reaction types, and the content type with the highest user engagement and score, providing valuable insights for Social Buzz. Additionally, slicers and timelines were added using the sentiment and datetime columns, respectively, to enhance data interactivity.


## Conclusion and Recommendation *****
 ***8The analysis revealed that "animal content category" received the highest user engagement with 1,897 reactions. *****The "super-love reaction" and "adore" was identified as the most prevalent, indicating strong positive audience sentiment. Futhermore, audio and photo content types ***** higher compared to videos and GIFs, highlighting format preferences. 
 
Recommendations include:
 1. Continue prioritizing content in the top-performing category (Animal Content).
 2. Given that the "super-love reaction" was the most commonly used, future content could be designed to elicit positive emotional responses from users, increasing overall engagement.
 3. Since "audio and photo content" perform best, Social Buzz Media should focus on optimizing these formats in future campaigns.
 4.  Regularly track engagement metrics over time to identify emerging trends and adjust the content strategy accordingly.



