# Data Analysis on NSF research grant text data

Hi! The motivation for this analysis was to use the data from the National Science Foundation website to inform researchers on what topic of research are in demand.

The questions to ask were, what areas of research are most sought-after? Among those topics, which offer the most funding? 

To conduct this project, I counted the frequency of research topics in the title and abstract section of the data and calculated the corresponding funding amount.


* **TASK_SUMMARY** 

  **Data Extraction:** The website text files were written in an XML file format, which had to be parsed and converted into a readable and workable dataframe.
  
  
  <img src="https://user-images.githubusercontent.com/89544848/153977136-2f32612d-2971-4cbf-aca6-be136cbecffe.png" width="250" height="250">
  
  <img src="https://user-images.githubusercontent.com/89544848/153977458-ee18d4dd-90f5-4686-b043-02ee889cd8c9.png" width="700" height="300">
  
  The parsed XML files are currently saved as CSV files.
  
   **Data Cleaning:** Next was data cleaning. 
   1. The data needed to remove any missing values. 
   2. I filitered non-research-related awards. 
   3. I remove stop words. 
   4. Removed additional irrelevant words

   **Data Analysis:** Here, I conducted various analysis on the data.
   1. NetworkX: Applied relation network to each key research topics to determine how one topic is related to the other, visualizing as a network of nodes.
   2. K-means clustering: Categorized the research topics based on the amount of funding each topics received.
   3. Machine Learning: Used Random Forest Model and XGBoost to predict the fundings for each research topic based on various metrics.
   4. Linear Regression: Analyzed the simple regression model and found the strength of the relationship by finding its coefficient of determination.

  



