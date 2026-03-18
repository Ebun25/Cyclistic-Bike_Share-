
# Cyclistic Bike-Share Analysis
# Project Overview
This project analyzes Cyclistic bike-share data to uncover behavioral differences between casual riders and annual members, with the goal of identifying strategies to convert casual riders into paying members.
The analysis was conducted using Python (Pandas) in Google Colab, focusing on data cleaning, transformation, and exploratory analysis to generate actionable business insights.

# Business Problem
This analysis aims to increase long-term revenue by converting casual riders into annual members.
This analysis answers:
    * How do casual riders and members differ in behavior?
    * When do riders use bikes the most?
    * Why would casual riders consider a membership?
    * How can Cyclistic use digital media to influence conversion?

# Dataset
The analysis uses historical bike trip data from Cyclistic, including datasets from different periods with different schemas.
Key fields include:
  * Ride timestamps (started_at, ended_at)
  * Station information (start and end stations)
  * Rider type (casual vs member)
    
# Tools & Technologies
  * Python
  * Pandas
  * Google Colab
  * Data Cleaning & Transformation
  * Exploratory Data Analysis (EDA)
  
# Data Cleaning & Preparation
To ensure consistency and accuracy, the following steps were performed:
  * Compared schemas across datasets 
  * Standardized column names between datasets
  * Selected shared columns for alignment
  * Merged datasets using pd.concat()
  * Converted datetime fields to proper format
  * Created new features:
      ride_length (duration of each ride)
      ride_length_minutes (converted for analysis)
      day_of_week
  * Removed invalid records:
      Negative ride durations
      Rides longer than 24 hours
  * Standardized rider categories:
      Customer → casual
      Subscriber → member

  # Key Findings   
  # Ride Duration Differences
  * Casual riders: ~36–41 minutes
  * Members: ~11–13 minutes
Observation: Casual riders take rides that are approximately 3× longer than members.

# Weekly Usage Patterns
  Member rides are concentrated on weekdays.
  Casual riders show increased activity on weekends.

# Behavioral Differences
Casual riders take longer, more of leisure rides that are more on weekends, whereas members take shorter, more routine trips during weekdays, consistent with behaviours.

# Business Insights
  * Casual riders are high-value users due to longer ride durations.
  * Weekend spikes suggest recreational use patterns.
  * Members exhibit consistent usage, indicating routine commuting behavior.
  * Casual riders with frequent weekend activity are strong candidates for membership conversion.

# Recommendations
  * Personalized In-App Messaging
    Show users potential cost savings based on ride behavior
    Target frequent and long-duration riders
  * Social Media Campaigns
    Highlight lifestyle and leisure benefits of membership
    Focus campaigns on weekend riders
  * Email & Push Notifications
    Provide ride summaries and cost comparisons
    Encourage conversion with data-driven insights
  * Promotional Offers
    Offer free trials or discounted memberships
    Target high-frequency casual riders

# Conclusion
The analysis reveals clear behavioral differences between casual riders and members. Casual riders demonstrate longer and more recreational usage patterns, while members exhibit shorter, routine trips.
By leveraging behavioral insights and targeted digital strategies, Cyclistic can effectively convert casual riders into annual members, increasing both retention and long-term revenue.

# Reference
This project is based on the Cyclistic case study from the Google Data Analytics Professional Certificate.


