# Social-Buzz-Project
## Introduction
This project involved working with a client in the media and content industry, where our objective was to analyze user reactions to various content categories. The aim was to identify the top 5 categories based on user interactions. As part of the analytics team, I was tasked with selecting the most relevant datasets, cleaning and transforming the data, and applying necessary functions like VLOOKUP and SUMIF to derive insights. The project emphasized data modeling and category-based performance evaluation for improving client recommendations and decisions.

## Problem Statement
The key challenge was to identify the top 5 content categories based on user engagement and popularity. To achieve this, we had to analyze user reactions across different datasets, clean and prepare the data, and derive category-wise performance metrics.

## Data Sources
 Out of the 7 datasets provided by the company, I identified 3 relevant datasets for analysis:
 1. Reaction Types: This dataset contained **3 columns and 17 rows**, details about the types of reactions, Sentiment, and score.
      ![Image](https://github.com/user-attachments/assets/3baf4fc8-76a5-4f50-8d52-5167be70001c)

 3. Reaction: Contained **5 columns and 25554 rows**, the reactions given by users to various content, including Content ID, user ID, types of reations, and datetime.

     ![Image](https://github.com/user-attachments/assets/0dcacea5-d837-4550-9ea3-455df22a52d6)
 
 5. Content: This dataset has **3 columns and 1001 rows**, captured details of the category about the content uploaded, including the content ID, content type and user ID.

     ![Image](https://github.com/user-attachments/assets/6608c7e2-5231-47db-943e-566253bc5c3c)

## Skills Demonstrated
1. Data Transformation: Converted each dataset into table, to make it look more structured. Cleaned and prepared the datasets by removing irrelevant columns such as user ID, URL, fixing column titles, and ensuring the data was consistent.

3. VLOOKUP Function: Used to merge data from the three datasets, with the reaction datasets serving as the primary base.
   
4. SUMIF Function: Applied to calculate the total reaction scores for each category, enabling us to rank categories based on scores.

5. Find and Replace Function: Employed to ensure consistency in the Category column, replacing repeated values for accurate analysis.

6. Sorting: Sorted the data by total reaction scores to identify the top 5 most popular content categories.

**First thing! I created a copy each of the original datasets as backup.**

## Data Transformation
1. Reaction Dataset:
   
   i. Converted the dataset to table, to make it look structured.
       ![Image](https://github.com/user-attachments/assets/2391fa17-cac6-4a55-9986-dc6d79314e84)

   ii. Deleted "column 1" that adds no information to the dataset, so also the "UserID column".
     ![Image](https://github.com/user-attachments/assets/9f371f91-f794-4cf8-9238-dff4fcfabbae)  ![Image](https://github.com/user-attachments/assets/c41a06f0-edd3-4efa-ae28-1e70948b94cc)

   iii. Using the filter function, filtered and deleted blank rows of the "type" column.
      ![Image](https://github.com/user-attachments/assets/ae5a85e1-941b-4cce-8ab6-fcec5a13067f)

   iv. Formatted column title of type to "Reaction type", making it more descriptive.   

    v. Used the **text** function to fornat the datetime column into date and time redpectively.
      ![Image](https://github.com/user-attachments/assets/2d28085d-77ad-415b-97ef-2ef940b896ce)

      ![Image](https://github.com/user-attachments/assets/0b266306-6d3c-4912-a044-ad8c983aab44)

Voila! The reaction dataset is cleaned and ready for analysis.
  
   ![Image](https://github.com/user-attachments/assets/c5914fdf-f1b3-4b17-83b3-0357512ca456)

2. Content Dataset:
   
   i. Converted the dataset to table, to make it look structured.
      ![Image](https://github.com/user-attachments/assets/dd1552cb-c2bf-45a5-8974-09ef0875a21e)

   ii. Deleted "column 1" that adds no information to the dataset, so also the "UserID" and "URL" column.
    
   iii. Formatted "Type" and "category" to "Content type" and "Content category" respectively.

   iv. There were inconsistencies in the "Content category",
   
     ![Image](https://github.com/user-attachments/assets/afae8a58-4857-4ed0-92db-56abdeba2f2c)

     Using the **Find & Replace function**, it was corrected to give the dataset a clean and final look.

     ![Image](https://github.com/user-attachments/assets/83787cae-ca41-4486-96d7-7c6787b1fc69)
   
   Ready for analysis!
   
     ![Image](https://github.com/user-attachments/assets/d02a30e8-fdc0-44ec-a88b-c2dab2a2c88b)

4. Reaction Types dataset:
   
   i. Converted the dataset to table, to make it look structured.
   
    ![Image](https://github.com/user-attachments/assets/fbe64dc9-9ec4-41ae-a6dd-fe19d35ac0a8)

   ii. Deleted "column 1" that adds no information to the dataset.
   
    ![Image](https://github.com/user-attachments/assets/8c4aa68d-4007-4e69-8496-7b675d7a4f85)
        
   iii. To make the field consistent, "type" column was formatted into "Reaction type"
 
    ![Image](https://github.com/user-attachments/assets/f5e5c632-e75a-4283-b09a-300454eea4d1)

Ready for analysis!

  ![Image](https://github.com/user-attachments/assets/f5e5c632-e75a-4283-b09a-300454eea4d1)
  
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



