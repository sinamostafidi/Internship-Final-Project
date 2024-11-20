# Internship-Final-Project
### The User Segmentation project involves analyzing a dataset containing user payment and demographic information for various services. The goal is to segment customers based on their behavior and generate actionable insights. The project utilizes Python for data preprocessing and Microsoft Power BI for visualization and dashboard creation.
## Python Section: Data Preprocessing and Cleaning
### 1. Loading the Data and Checking Structure
### •	Load the dataset using pandas and inspect its structure (e.g., info(), head(), describe()).
### •	Check data types, null values, and overall summary.
### 2. Finding Duplicate Columns
### •	Identify and drop duplicate columns based on their content to avoid redundancy.
### 3. Replacing Outliers with NaN
### •	Use statistical methods (e.g., IQR or z-scores) to detect outliers in numerical columns.
### •	Replace detected outliers with NaN for further processing.
### 4. Analyzing Missing Values
### 4.1. Calculating the Percentage of Missing Values
### •	Compute the percentage of missing values for each column to understand data quality.
### 4.2. Identifying Columns with High Missing Rates
### •	Flag columns with over 70% missing data for potential removal.
### 5. Handling Missing Values
### 5.1. Dropping Columns with More Than 70% Missing Values
### •	Eliminate columns that lack sufficient data to maintain dataset quality.
### 5.2. Dropping Rows with More Than 50% Missing Values
### •	Remove rows where over half of the columns have missing values.
### 6. Imputation Methods
### 6.1. Datetime Columns (Forward Fill)
### •	Use forward-fill (ffill) to fill missing values in datetime columns, ensuring chronological consistency.
### 6.2. Numerical Columns (K-Nearest Neighbors)
### •	Apply KNN imputation to fill missing numerical values based on similar observations.
### 6.3. Categorical Columns (Mode Imputation)
### •	Replace missing values in categorical columns with the most frequent value (mode).
### 7. Data Type and Calendar Type Correction
### •	Convert FirstTrsDate and LastTrsDate from Gregorian to Jalali calendar.
### •	Ensure proper formatting for datetime columns.
### 8. Saving the Processed Data
### •	Save the cleaned and preprocessed dataset to an Excel file for further analysis.
## Microsoft Power BI Section: Visualization and Analysis
### 1. Checking All Columns
### •	Validate the structure, data types, and content of each column to ensure data integrity.
### 2. Creating Metrics
### •	Generate key metrics to describe user behavior and performance:
### o	Recency: Days since the last transaction.
### o	Frequency: Number of transactions.
### o	Monetary: Total monetary value of transactions.
### o	AvgServiceUsage: Average number of services used.
### o	SuccessRate: Ratio of successful transactions.
### o	AppErrorRate: Application-related errors as a percentage of total transactions.
### o	UserErrorRate: User-induced errors as a percentage of total transactions.
### o	BalanceErrorRate: Balance-related errors as a percentage of total transactions.
### o	RFM_Segment: RFM segmentation score.
### o	Age: User’s age derived from birthdate.
### o	UniqueServices: Number of unique services used.
### 3. Creating Segmentation Columns
### •	Add segmentation columns to categorize users based on RFM analysis:
### o	Recency Segment
### o	Frequency Segment
### o	Monetary Segment
### 4. Creating Charts ; Visualize key insights through the following charts:
### 4.1. Count of Recency Segment by Recency Segment
•	Show the distribution of users across recency segments.
![image](https://github.com/user-attachments/assets/62cc838b-e093-42c0-95e7-4c9a8d6d073e)
### 4.2. Count of Frequency Segment by Frequency Segment
•	Display the frequency distribution of user transactions.
![image](https://github.com/user-attachments/assets/c2d2d37b-e419-403d-b13b-f1517f14a305)
### 4.3. Count of Monetary Segment by Monetary Segment
•	Analyze monetary contribution distribution among users.
![image](https://github.com/user-attachments/assets/18eb9822-97df-414c-b649-e1aa7136c3ba)
### 4.4. Count of Person Gender Title by Age and Person Gender Title
•	Explore age and gender demographics.

![image](https://github.com/user-attachments/assets/b390352a-37d5-46df-93f3-cdbbfee099a2)
### 4.5. Unique Services by Top Service
•	Identify top-used services by unique users.
![image](https://github.com/user-attachments/assets/136ca9ff-ad16-4185-8186-5a3012c01378)
### 4.6. Count of Mobile Device Brand by Mobile Device Brand
•	Show the distribution of users by mobile device brand.
![image](https://github.com/user-attachments/assets/506b8627-6603-4cdb-a298-1b0a572e271a)
### 4.7. Count of Mobile Device Model by Mobile Device Model
•	Analyze user distribution by device model.
![image](https://github.com/user-attachments/assets/bdf7951c-e49f-4e1b-9b4c-575ea86362d2)
### 4.8. Count of Mobile Device OS Title by Mobile Device OS Title
•	Explore operating system preferences.

![image](https://github.com/user-attachments/assets/45d5303d-5724-4404-802a-435337e3b9da)
### 4.9. Success Rate, User Error Rate, App Error Rate, and Balance Error Rate
•	Evaluate transaction success and error rates.
![image](https://github.com/user-attachments/assets/072bdd2c-791a-4c9c-855e-f70eeb6bb004)
### 4.10. Comparing Error Ratios
•	Compare different error rates (User, App, Balance) and success rates.
![image](https://github.com/user-attachments/assets/0762df30-6b74-492a-9bb7-9e39ac471499)
### 4.11. Count of First App Install Date by Year
•	Visualize user acquisition trends over time.
![image](https://github.com/user-attachments/assets/cb637223-7883-4d4a-8c94-5401f0296a7d)
## Insights 
### 1. User Activity Insights
### •	Recency Analysis (4.1):
### o	Recent Users: 12.1K users have interacted with the platform recently, indicating strong engagement.
### o	Dormant Users: 9.5K users show a decline in engagement, suggesting the need for re-engagement strategies.
### o	Inactive Users: 2.7K users are completely disengaged, requiring targeted retention or win-back campaigns.
### •	Frequency Analysis (4.2):
### o	Infrequent Users: 12.1K users have minimal interaction, reflecting potential for upselling or encouraging higher usage.
### o	Moderate Users: 9.2K users represent a steady usage pattern, possibly due to balanced needs.
### o	Frequent Users: 3.0K frequent users are likely power users who contribute significantly to platform activity.
### •	Monetary Analysis (4.3):
### o	Low-Value Users: 12.2K users contribute minimally to revenue, highlighting opportunities for monetization strategies.
### o	Medium-Value Users: 11.0K users form the majority of mid-tier customers, which can be a stable revenue base.
### o	High-Value Users: 1.1K users are key contributors to revenue, requiring personalized attention and retention strategies.
### 2. Demographics and Behavior Insights
### •	Demographics (4.4):
### o	Gender: The majority of users are male.
### o	Age: Most users are aged between 25-40, with 35 being the most common age. This indicates a target audience of young to middle-aged adults.
### •	Top Services (4.5):
### o	The most popular services are C2C Transfers, followed by ChargeMCI, ChargeMTN, ETC, and others.
### 	Actionable Insight: Focus on enhancing these services and cross-promoting lesser-used services to increase adoption.
### 3. Device and Platform Insights
### •	Mobile Brands (4.6):
### o	Top 3 Brands: Samsung, Xiaomi, and Huawei dominate the user base.
### 	Actionable Insight: Optimize app performance for these brands and prioritize compatibility testing.
### •	Device Models (4.7):
### o	The most common models are Samsung SM-A107F, Redmi Note 8, and Samsung SM-A325F.
### 	Actionable Insight: Ensure seamless app functionality on these models to enhance user experience.
### •	Operating Systems (4.8):
### o	Android Users: 22.6K dominate the platform.
### o	PWA Users: 1.5K rely on progressive web apps.
### o	iOS Users: 0.2K are minimal, indicating low engagement on Apple devices.
### 	Actionable Insight: Focus on Android optimization and consider strategies to increase iOS user engagement.
### 4. Performance Metrics
### •	Success and Error Rates (4.9):
### o	Success Rate: 82% of transactions are successful, showing reliable system performance.
### o	User Error Rate: At 1%, it indicates a manageable level of user mistakes.
### o	App Error Rate: At 3%, improvements can enhance reliability further.
### o	Balance Error Rate: Almost negligible at 0%.
### 	Actionable Insight: Focus on reducing app errors through updates and user-friendly interfaces.
### 5. User Acquisition Trends
### •	First App Install Date (4.11):
### o	Peak Year: 2018 with 4.7K users, likely due to effective campaigns or service introduction.
### o	Minimum Year: 2014 (the platform's launch year) with only 0.2K users.
### o	Recent Year: 2023 saw a decline to 0.8K users.
### 	Actionable Insight: Evaluate and revamp acquisition strategies to regain momentum in user onboarding.
## Overall Strategic Recommendations
### 1.	Engagement and Retention:
### o	Re-engage dormant and inactive users through targeted marketing and personalized offers.
### o	Encourage infrequent users to increase transactions with loyalty programs or usage incentives.
### 2.	Revenue Growth:
### o	Focus on converting low-value users to medium- or high-value segments through promotions and tailored recommendations.
### 3.	Service Optimization:
### o	Invest in the enhancement of top-used services and cross-promote lesser-used ones.
### 4.	Platform Performance:
### o	Optimize for Android users and focus on resolving app errors to improve user satisfaction.
### 5.	User Acquisition:
### o	Analyze factors behind the 2018 peak and replicate successful strategies to boost future growth.

