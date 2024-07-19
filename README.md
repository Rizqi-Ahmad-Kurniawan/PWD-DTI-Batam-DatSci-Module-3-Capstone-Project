# PWD-DTI-Batam-DatSci-Module-3-Capstone-Project

# ✨✨✨ Capstone_Project_3_Purwadhika ✨✨✨

# California Housing Price


## Presentation (visual overview)
- California Housing Price ML Model Presentation Link: https://drive.google.com/drive/folders/1JyzDvG0GnRwilZYmARtjxKW50G1XIA-O?usp=drive_link 
- California Housing Price ML Model - Google Cloud Platform - Link: https://shell.cloud.google.com/?hl=en_US&authuser=1&fromcloudshell=true&show=terminal
- ML Model Medium (article) Link: https://medium.com/@rizqikurniawan233/from-data-to-deployment-a-brief-guide-to-building-your-first-machine-learning-model-b1967bf89e5a 

## Quick Overview
- Capstone project for learning module 3 of Purwadhika DTI Data Science Program. 
- The project is a Machine Learning Model that is trained on a dataset that contains California's Housing Price information (and complementary variables) from the 1990 California census 

![image](https://github.com/user-attachments/assets/7d951ee3-0d78-486f-82e9-6e1e9a182a06)


## General Overview

## 1. Business Understanding

### ===== Context (Background) =====

* **History:** California is a state located on the southwest coast of the United States. Known as "The Golden State", California has a very rich history, geography and culture. Here are some important points regarding California's background:<br>

    **California 1990 :**

    * **Economy:** In 1990, California had a rapidly growing economy, supported by the technology, agriculture, entertainment, and manufacturing sectors. Silicon Valley, in the San Francisco Bay Area, has become a global technology center, and technology companies such as Apple and Microsoft play a large role in economic growth.

    * **Population:** California's population in 1990 had reached more than 29 million residents. As the economy grew, many residents from various states of the United States and abroad moved to California.

    * **Culture:** California continues to promote cultural diversity, arts and entertainment. By 1990, the entertainment industry in Hollywood had long been the center of world film and television production.

    * **Environment:** California in the 1990s faced environmental challenges, including drought and air pollution problems. Conservation and environmental protection efforts are increasingly becoming a major concern.
    
* **Context:** The data contains information from the 1990 California census. So, although it may not help with predicting current housing prices, it does provide an accessible introduction dataset for "1990 California Housing Price" using Machine Learning.
* **Background:** The goal of the "Business Understanding" phase is to comprehend the project objectives and requirements from a business perspective, and then convert this knowledge into a data mining problem definition and a preliminary plan designed to achieve the objectives. California's real estate market is one of the largest and most dynamic in the United States. Factors influencing house prices include location, proximity to amenities, socio-economic factors, and market conditions. Accurate prediction models can provide significant value to stakeholders (Individuals or Groups, or Enterprises) in the real estate industry.
* **Acknowledgement:** This data was initially featured in the following paper: Pace, R. Kelley, and Ronald Barry. "Sparse spatial autoregressions." Statistics & Probability Letters 33.3 (1997): 291-297.


### ===== Problem Statement =====

* **Problem:** Individuals, Groups, or Enterprises have a harder time predicting House Prices in California for the year 1990. Stakeholders (sellers & buyers) wants to save their time, lower costs, and have transactions with better price-to-value ratio for a fairer and more efficient market
* **Solution:** Create an ML Model that is able to predict House Prices accurately for House prices in California in the 1990s


### ===== Data Understanding =====
<img width="895" alt="Screenshot 2024-07-19 at 17 53 39" src="https://github.com/user-attachments/assets/58537b7f-e8ea-418a-b513-acf3bd2166e5">


### ===== Goals =====

#### ===== Project Goals =====

1. **Macroeconomic Perspective:**
    1. Increasing Economic Market Efficiency through “Price Equilibrium” (balancing supply and demand)
    2. The Potential for more “Transaction Quantity” and “Amount Transacted” -> increasing Gross Domestic Product (i.e. more prosperous)
2. **Seller’s Perspective:** 
    1. Higher “Capital Gain” from optimal pricing 
    2. More “Time saved” by potentially having the property be sold faster (less dormant/idle time)
    3. More “Money saved” by reducing expenses on “Housing price Market Research” due to the research process requiring only an internet access to access the ML Model in discussion instead of the “Manual” way to do market research/surveys
3. **Buyer’s Perspective:**
    1. Better “Property Deals” that suits their respective “Price : Value” ratio perspective 
    2. More “Time saved” by potentially finding a property faster through the “correct” pricing (less research/exploration time)


#### ===== General Benefit =====

1. **Understand Market Trends:** By predicting house prices, we can identify trends of price increases or decreases in specific regions based on the independent and dependent variables present. This information assists both buyers and sellers in making informed decisions.
2. **Financial Planning:** Price predictions enable individuals and families to plan ahead their home purchases wisely. For instance, knowing the estimated future house prices aids in savings and financing planning.
3. **Property Investment:** For investors, predicting house prices helps in selecting potentially profitable properties. Understanding the factors influencing prices allows for smarter and more informed decision-making.
4. **Housing Policies:** Governments and related institutions can use house price predictions to design effective and sustainable housing policies that caters to inclusivity whilst upholding fair and healthy market pricing.


#### ===== Project Implementation =====

1. **Property Market App/Web:** App/Web can connect through our API to access our ML Model and help with predicting the Property Prices Listed on the app/web. Given the Features (independent variables) are common and resembles the market condition.
2. **Property Developer Enterprise:** Enterprises can utilise our API to access our ML Models and help plan their Property Development by knowing the prices in advance, helping them in finding the Optimal Operational Budget for development purposes. Given the Features (independent variables) are common and resembles the market condition.


### ===== Analytical Approach (Models and Evaluation Metrics) =====

* **Intro:** The analytical approach that we will apply is to carry out data analysis by identify patterns from the available data. We will develop a **Machine Learning using Regression models**. This model will help property owners, both individuals and companies, in determining the optimal selling price for apartments.
* **Models:** Linear and Non-Linear (alternative when performance is still poor) Regression
* **Evaluation Metrics:** The Evaluation Metrics that we are going to utilise are RMSE, MAE dan MAPE. The smaller the metric's value (as it nears to 0), the more accurate the model.


* **[1] RMSE (Root Mean Square Error)**
RMSE is one of the evaluation metrics commonly used in regression problems to measure the extent of the difference between the predicted values ​​from the model and the actual values ​​from the data. RMSE measures the average of the squared differences between each prediction and the actual value, then takes the square root. This gives an idea of ​​how big the deviation or average error of the model predictions is to the actual value.

The RMSE formula is as follows:
<br>
![image-3.png](attachment:image-3.png)
<br>
    - ∑ is sigma (the sum of a sequence or function)<br>
    - ŷi is the predicted value of data i<br>
    - yi is the actual value of data i<br>
    - n is the number of data<br>

* **[2]MAE (Mean Absolute Error)**
MAE is used as an evaluation metric because it has several advantages, especially when used in the context of predicting prices as in this case:
1. Not Sensitive to Outliers: MAE is not very sensitive to outliers, so if there are some extreme values ​​in the data, MAE still provides a good idea of ​​how well your model predicts most of the data.
2. Suitable for Price Prediction: MAE is suitable for use in the case of price prediction because prices often have a large range of values, from units to billions. MAE does not give greater weight to larger price differences, so it is useful for measuring prediction errors on a uniform scale.

The MAE formula is as follows:
<br>
![image.png](attachment:image.png)
<br>
    - ∑ is sigma (the sum of a sequence or function)<br>
    - ŷi is the predicted value of data i<br>
    - yi is the actual value of data i<br>
    - n is the number of data<br>

* **[3] MAPE (Mean Absolute Percentage Error)**
MAPE is an evaluation metric used to view the error in terms of a percentage of the true value. This gives an idea of ​​the extent to which Machine Learning predictions are close to the actual values ​​in percentage form.
1. Evaluation in Percentage Form: MAPE measures the prediction error in percentage terms, which allows us to assess the level of accuracy of the model relative to the actual price.
2. Suitable for Price Prediction: MAPE is suitable for use in the case of price prediction because prices generally do not have a value of 0, so MAPE being sensitive to the value of 0 is impossible in this case.

The MAPE formula is as follows:
<br>
![image-2.png](attachment:image-2.png)
<br>
    - ∑ is sigma (the sum of a sequence or function)<br>
    - ŷi is the predicted value of data i<br>
    - yi is the actual value of data i<br>
    - n is the number of data<br>


### ===== Model Limitations =====

* The Model is only designed to **predict** house prices for a **specific circumstance/setting:**
    * **Location:** California, USA
    * **Time:** 1990
    * **Specifics:** based only on a single dataset from the  following paper: Pace, R. Kelley, and Ronald Barry. "Sparse spatial autoregressions." Statistics & Probability Letters 33.3 (1997): 291-297.
* **Disclaimer:** Any Predictions made **outside** of the required and intended context should **not** be subjected as **reference**
