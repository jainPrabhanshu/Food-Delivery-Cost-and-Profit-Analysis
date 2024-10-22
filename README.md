# Food-Delivery-Cost-and-Profit-Analysis

## Preview of the Dashboard (Power BI Service)

![image](https://github.com/user-attachments/assets/334b05f1-cf0d-483d-8454-a51c9c3b5f4e)

![image](https://github.com/user-attachments/assets/33890e9a-c68c-41bd-acd2-8f4164c4ab29)

![image](https://github.com/user-attachments/assets/d0c21292-5743-4f4f-8110-d37dfa2526da)

![image](https://github.com/user-attachments/assets/cd0ad5b0-19b3-45c0-8a33-41d3cf66dd3e)

![image](https://github.com/user-attachments/assets/c5ece960-6765-48b4-8582-c8f268145cce)

## Problem Statement

In the highly competitive food delivery market, managing costs and maintaining profitability is critical for businesses. Delivery fees, commissions, and operational expenses can directly impact profitability, making it essential to analyze key metrics such as order values, delivery fees, commission rates, and payment methods. This project aims to develop an interactive Power BI dashboard to provide insights into delivery costs, profitability by restaurant, order trends, and customer behavior. 

### Project Goals

-  Profitability Analysis : Measure profits per restaurant, per order, and by time period (daily/monthly).
  
-  Delivery Cost Insights : Analyze the impact of delivery fees and commission rates on profitability.
  
-  Customer Behavior : Understand order patterns by analyzing customer preferences in payment methods, peak order times, and delivery durations.
  
-  Restaurant Performance : Identify the top-performing restaurants based on order value, delivery fees, and profitability.
  
-  Interactive Visualizations : Enable users to filter data by restaurant, order date, payment method, or delivery fee for detailed insights.

## Data Source
The data used for this project was sourced from internal delivery records. It contains information on :

[Food Delivery Cost and Profitability](https://www.kaggle.com/datasets/romanniki/food-delivery-cost-and-profitability)

  - ### Data Preprocessing Involved

      - #### **Data Cleaning**

          - Handling missing values: Identified and removed rows with missing or incomplete data (e.g., null customer IDs or delivery times).
          - Removing duplicates: Eliminated any duplicate orders from the dataset.
          - Standardizing text data: Fixed inconsistent naming of restaurants, payment methods, and delivery statuses. 

      - #### **Data Transforamtion**

          - Converted order dates and delivery times to appropriate datetime formats for time-based analysis.
          - Identified outliers in order values and delivery fees, which were transformed to ensure they didn’t skew analysis.
          - Created new calculated fields such as
              - Total Cost = Delivery Fee + Commission Fee + Payment Processing Fee
              - Profit per Order = Order Value – Total Cost

      - #### **Data Integration**
  
          - Merge data from different sources (if applicable): For example, combine historical Olympic data with the 2024 dataset to analyze trends.
    
      - #### **Data Validation**

          - Check for consistency: Ensure the cleaned data aligns with known facts (e.g., no country has more medals than events they've participated in).

## Steps Followed 

- Step 1 : Load the dataset onto Power Query Editor.

- Step 2 : Data transformation based on the requirements. Included steps like creating tables like Date, Measures and other metrices.

- Step 3 : Created the following measures to extract key statistics from dataset:

    ![image](https://github.com/user-attachments/assets/d8d27d30-7fd4-478f-8594-eb99d0577efc)

- Step 4 : Rectified the Relational Model by linking Primary keys, foreign keys and updating table cardinalities.
    ![image](https://github.com/user-attachments/assets/cf68a58f-3902-450b-a8a9-f5ccaacbc9b8)

- Step 5 : Visualized the dashboard structure based on three key questions:
       
        Q1. What type of data is being dealt here?
         Ans. Time series data, categorical, geospatial and hierarchical.

        Q2. What am I trying to communicate here?
         Ans. Comparison between categories over time, depicting compositions.

        Q3. Who is the end-user?
         Ans. The Viewers           


- Step 7 : Created three pages to provide different insights to the viewer:
    
    - #### Overview insights
    - #### Athletes insights
    - #### Country insights
    - #### Historical insights

- Step 8 : The dashboard was complete with all my target requirements being met. Finally, I linked all the pages using Buttons to facilitate smooth navigation.

- Step 9 : Uploaded the entire Dashboard to PowerBI Service.

## Key Insights from Olympics 2024 Data Analysis

1. Medal Distribution by Country
    - The top 5 countries (USA, China, Russia, Japan, and Germany) dominated the medal tally, collectively winning over 50% of the total medals.
    - Smaller countries like Jamaica and Kenya continue to excel in specific events such as athletics, particularly in sprint and long-distance running.

2. Gender-Based Analysis
    - Women athletes contributed nearly 45% of the total medals, showing a growing trend toward gender equality in participation and performance.
    - Certain events, such as gymnastics and swimming, saw near-equal participation and performance by men and women.

3. Most Successful Athletes
    - Key athletes like Caeleb Dressel (USA, Swimming), Elaine Thompson-Herah (Jamaica, Track), and Simone Biles (USA, Gymnastics) were the most successful, winning multiple gold medals and contributing significantly to their country’s overall success.
  
4. Trends Over Time
    - Analysis of historical data shows an upward trend in the total number of participating countries and athletes, with a record number of women participants in 2024.
Over the years, the gap between top-performing and developing countries is narrowing, particularly in sports like badminton and wrestling.

## Challenges Faced During the Olympics 2024 Project

1. Data Limitations:

    - Incomplete Data: Some datasets were missing critical information like athlete names or detailed event results, requiring manual data entry or external sources for completion.
    - Inconsistent Data Formats: Different datasets (e.g., historical data vs. 2024 data) had varying formats for country names, event types, and medal categories, making integration and analysis difficult.
    - Lack of Real-Time Data: Some real-time data, such as live updates on event results, were not available or lagged, limiting the ability to capture the latest insights.
  
      
2. Technical Issues:

    - Data Cleaning Complexity: Handling a large and diverse dataset required extensive data cleaning, particularly with missing values and duplicate records, which was time-consuming.
    - Performance Bottlenecks: The large size of the dataset sometimes caused Power BI to slow down, especially when applying multiple filters or handling complex visualizations.
    - Data Merging: Integrating multiple datasets (e.g., historical and 2024 event data) posed technical challenges, such as ensuring alignment of common fields and avoiding data redundancy.

## Future Improvements for Olympics 2024 Data Analysis Project

1. Real-Time Data Integration: Incorporate real-time data feeds to update the dashboard instantly with live event results, medal counts, and athlete performance, offering more dynamic and current insights.
2. Predictive Analytics: Implement machine learning models to predict future outcomes, such as likely medal winners or country performance trends based on historical and current data.
3. Deeper Athlete-Level Analysis: Expand the dataset to include more granular data on individual athletes, such as personal best performances, injury history, and seasonal form, for more detailed performance evaluations.
4. Additional Visualizations: Add interactive and advanced visualizations, such as heat maps to track country-wise performance across regions or animated time-series charts to highlight historical trends in medal counts.
5. Incorporating Audience and Social Media Data: Integrate social media mentions, audience engagement, and public sentiment analysis to evaluate the popularity of different sports, athletes, and events throughout the Olympics.
6. Optimization for Large Data: Improve dashboard performance when handling large datasets by optimizing data models, reducing file size, and incorporating efficient query techniques for smoother user experience.

## License

This project is licensed under the [MIT License](LICENSE).

