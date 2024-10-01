# **Swiggy Delhi Restaurant Analysis**

## **Project Description**

This project analyzes restaurants in Delhi listed on Swiggy, focusing on various features such as cuisine type, location, ratings, and price for two. The goal is to derive insights into restaurant trends, popular cuisines, and the distribution of ratings and prices across different locations in Delhi.  

## **Dataset Information**

The dataset contains 912 rows and 6 columns, with the following fields:

**name:** Name of the restaurant (e.g., Momo Maker, Moets Kulfi)  

**cuisine:** Type(s) of cuisine the restaurant serves (e.g., Snacks, Tandoor, Desserts)  

**location:** Location of the restaurant (e.g., Lajpat Nagar, Defence Colony)  

**rating:** Restaurant rating (e.g., 4.7, 4.6, or -- for too few ratings)  

**num_of_rating:** Number of ratings (e.g., 50+ ratings, 1K+ ratings, or Too Few Ratings)  
**price_for_two:** Price for two people (e.g., ₹200, ₹500) 


### Sample Data
| Name                                  | Cuisine               | Location                              | Rating | Number of Ratings | Price for Two |
|---------------------------------------|-----------------------|---------------------------------------|--------|------------------|---------------|
| Momo Maker                            | Snacks, Tandoor       | Central Market, Lajpat Nagar          | 4.7    | 20+ ratings      | ₹200          |
| Moets Kulfi                           | Desserts, Beverages   | Defence Colony Market, Defence Colony | 4.7    | 50+ ratings      | ₹200          |
| Behrouz Biryani - Royal & Safe       | Biryani, Mughlai      | Near Metro Station, Shakarpur Khas   | 4.7    | 1K+ ratings      | ₹500          |
| Triveni Terrace Cafe                 | Indian                | Opposite FICCI Auditorium, Mandi House| 4.7    | 50+ ratings      | ₹400          |
| Momo Guy                              | Chinese, Tibetan      | GTB Nagar, GTB Nagar                  | 4.6    | 20+ ratings      | ₹200          |


  
  ### **Preprocessing

  Before analyzing the Swiggy restaurant dataset, several preprocessing steps were performed to ensure data quality and relevance:  

**Drop Duplicates:** The dataset was checked for duplicate entries, and any duplicates were removed to maintain the integrity of the analysis.  

**Identify Most Visited Locations:** An analysis was conducted to identify the locations with the highest number of restaurants. This helps in understanding the most popular areas for dining in Delhi.  

**Determine Preferred Cuisines: **The dataset was analyzed to find out which cuisines are most preferred by customers based on the number of restaurants available for each cuisine type.  

**Find Best Cuisine by Rating and Location:** To determine the best cuisine in terms of ratings within each location, a grouped analysis was performed, calculating the average rating for each cuisine type across different locations.  


### Data Visualization

Data visualization was performed using Plotly Express to create insightful graphics that help interpret the analysis effectively:

**Top 9 Locations by Cuisine:** A bar plot was created to visualize the top 9 locations with respect to the number of cuisines available. This visualization helps to identify areas with diverse dining options.  

**Top 15 Restaurants: **A bar chart displaying the top 15 restaurants based on ratings was generated to showcase the highest-rated establishments in the dataset, providing valuable insights for potential customers.  

**Count vs Cost for Two People:** A scatter plot was created to visualize the relationship between the count of restaurants and the cost for two people. This visualization highlights pricing trends in the restaurant industry, helping consumers make informed decisions.  

**Top 10 Locations of Restaurants:** A bar chart was plotted to show the top 10 locations ranked by the number of restaurants. This provides insights into the dining landscape of Delhi and indicates areas with a high concentration of dining options.  