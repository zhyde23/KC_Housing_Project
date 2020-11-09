# King County  Housing Project

## Introduction
During the analysis of data, I will be presenting to sell by owner's who want a better idea on what their property value is estimated at within the King County market of Massachusetts. Throughout this notebook, I will be explaining step-by-step what each section of code represents. My goal is to gain your business and trust in my  abilities to accurately utilize machine learning and linear regression modeling to predict your property value based on multiple variables (i.e. # bedrooms, # bathrooms, living sqft, etc).

## Objective
Utilizing the dataset provided, clean and explore the information and manipulate it to train a multiple linear regression model to accurately predict new information as it is recieved based on features alone. 

## KC Housing Data
The data consisted of 21,597 listings. Within those listings, there were 20 different variables describing each listing. As one would assume, the basics were square footage of living space, # bathrooms, # bedrooms, year built and listing price. The features that might not be so common were waterfront, year it was renovated, grade value based on the what the county scored it as, overall condition and different ways of describing the location. Among these features, I found that it was most benefitial to utilize: # of bedrooms, grade, waterfront (or view), condition, sqft of living space, year built, year it was renovated and lastly price to distinguish and predict what a new listing would be valued at because these features had the most significant impact on the model being used.
## Hypotheses
H0: The square footage of a property will not have a significant increase of the price.

H1: The square footage of a house will have a significant increase of the price.
_________________________________________________________________________________________________________________

H0: Having a waterfront feature will not increase the value of the property.

H1: Having a waterfront feature will increase the value of the property.
_________________________________________________________________________________________________________________
H0: The newer the building is, the higher the value.

H1: The older the building is, the higher the value.
## Conclusion
I can reject the null hypotheses. The coefficients to my hypothesis values are as followed: 'sqft_living'(200.487), 'h2ofront'(753,500) and 'yr_built'(-4000) with their p-values > 0.05. The final OLS model also shows that my R-squared value is 0.645 which is reflective of what my linear accuracy score shows of 65%. In summary, the more square footage you add to the living space of a property will increase the value 200 dollars; if you have a waterfront property, your value will rise 753,500 dollars and each year your house ages, it decreases value by 4,000 dollars.

## File Details within the Repository
* kc_house_data.csv -- data utilized to train model to predict prices to new listings based on specific features
* column_names.md -- description of what each column represents of the kc_house_data.csv
* Mod2 Scratchbook.ipynb -- Original notebook used to begin this project (includes code block not utilized for final modeling submission)
* KC Housing Project-Final Submission -- Final Draft of code includes: EDA/cleaning, testing simple linear regression, multiple linear regression, OLS tables, finding Root Mean Squared Error (RMSE) of different models, train-test spliting, and conclusion of findings. 
