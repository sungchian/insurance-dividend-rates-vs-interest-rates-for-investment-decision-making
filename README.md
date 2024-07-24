# 🎯 Project Objective 

This project is to create a visualization or series of visualization that analyze the relationship between the dividend rates of New York Life, Guardian Life, and MassMutual and U.S. government interest rates from 1990 to 2024.
My goal is to identify trends, correlations, and insights that assist in evaluating the performance of these insurance companies under various interest rate scenarios.

# 🔍 Data Requirements

Dividend rates from New York Life, Guardian Life, and MassMutual from 1990 to 2024 [Dataset](https://topwholelife.com/whole-life-insurance-dividend-rate-history/).

U.S. government interest rates from 1990 to 2024 [Interest Rates](https://fred.stlouisfed.org/series/FEDFUNDS#0).

# 📊 Data Visualization

- Time Series Line Chart:
    - Display dividend rates of New York Life, Guardian Life, MassMutual, and U.S. government interest rates on the same chart.
    - Use different colors for each company and government rate.
    - X-axis: Years (1990-2024), Y-axis: Rate percentage.
  <br>
      <img src="Images/dividend-rate-vs-interest-rate.png" width="500">
  <br> 

# 📈 Exploratory Data Analysis  
- The presence of outliers is evident, particularly in features like bed, bath, acre_lot, and house_size.
- The average property listing was priced at $886,657 with a standard deviation of over $2M indicating a large distribution range.
- There are missing values in the dataset that inaccurately represent some listings.
- The data represents a wide range of states that cover the Eastern, Mid-Atlantic, and Caribbean territories. As shown in the bar chart below, New York and New Jersey are the states that account for over 500,000 listings combined, followed by Massachusetts with approximately 175,000 listings.    
   <br>
      <img src="Images/img-01.png" width="500">
   <br>  
- The variables bed, bath, and house_size are positively correlated to price, meaning that the property price tends to increase as these features increase, as shown in the heat map below. (The redder the square, the weaker the correlation. The darker the gray or black, the stronger the correlation.)  
   <br>
      <img src="Images/img-02.png" width="500">
   <br>  
- In this dataset, New York appears to be the state with the highest average property price at over $1.4 million, whereas West Virginia appears to be the state with the lowest average property price, averaging around $62,000 per property. Additionally, the property price seems to increase in high-density urban areas such as New York City and parts of Boston, as shown in the map below.  
   <br>
      <img src="Images/img-03.png" width="500">
   <br>  
- Though New York and Massachusetts share similarities with their high average listing price, the features of these properties differ significantly. On a city-by-city comparison, the average house size in Massachusetts is much larger than that of New York. The smaller property size combined with the high price makes New York the state with the highest average price per square foot in this dataset.  
   <br>
      <img src="Images/img-04.png" width="500">
   <br>
- Georgia, West Virginia, and the Virgin Islands seem to have the highest average number of bedrooms and bathrooms per property.
   <br>
      <img src="Images/img-05.png" width="500">
   <br>

Highlighting these relationships helped us gain a deeper understanding of the data which offered valuable insight as we continued our analysis through machine learning models.  

# 👣 My Approach  




# 🔑 Key Takeaways    
We implemented three machine learning models to predict whether a real estate listing could be classified as a "high" or "low" price listing. From our analysis, we concluded how different models reacted to a variety of pre-processing techniques. From our choice of pre-processing techniques, the best techniques seemed to involve a combination of random sampling, standardization, and dummy variables for the state attribute. The binning technique improved the Logistic Regression model significantly. However, binning also led to a significant decrease in the performance of the Random Forest and KNN models, suggesting the importance of retaining the original granularity for some features.  

For this dataset, the best model seemed to be the Random Forest algorithm with no pre-processing. This model had the highest accuracy of 92%. Property location also seemed to be the attribute that plays a significant role in price.  

# ☁️ Project Improvements  
This project was for the first machine learning class that I took, and it was also the first project where I applied machine learning algorithms. Knowing what I know now if I were to improve this project, I would focus on improving the Random Forest model using different boosting methods, such as Adaptive Boosting and Gradient Boosting.  


 
