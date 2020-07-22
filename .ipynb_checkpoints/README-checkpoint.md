# WNBA Average Game Analysis

### Problem Statement: 
Negotiating contracts is already tough enough, but when working with professional athletes there are many factors to consider. The league and the athlete both want to leave feeling like they are receiving the best end of the deal. Houston Analytics, LLC. carefully analyzes each player's potential earnings with predictive modeling techniques. We take in to consideration their playing history and statistics to come up with the right answers for you. Our team is able to craft the best algorithms with feature engineering and analytic metrics that pair perfectly with our chosen model, to project the future of your player. 

### Proposed Deliverables:
When athletes are in season, their focus is being the best player they can be and increasing their personal stats. While they continue to be the best, our focus is to highlight the areas in which they are excelling and in need of improvement to assist them in becoming better every day. At Houston Analytics, we like to focus on longevity of your players. Our intention is to predict the average number of games your player can expect to play over an extended amount of time, taking into consideration all influencing factors from their team, position, defensive versus offensive contributions. Our philosophy here is that you can never have too much data nor enough guidance. The Average Game Analysis Project is one that will allow all parties involved in the contracting process to be well-informed with the latest on the athletes they are considering. 

### Executive Summary:
Supporting our athletes is a full time job because the data is always changing and there area so many avenues to explore in the world of sports. The Houston, Analytics team was tasked with calculating the minimum number of games a first year WNBA player is expected to play in the upcoming 3 years, given a distinct set of statistics to compare and engineer as we see fit.


**Linear Regression Model Scores:**
We ran a Linear Regression model then supplemented that with regularization usisng Ridge and LASSO. All variatons of the model not perform well with a 0.67 as the highest R2 Score for our testing data set.

Linear Regression Train R2 Score: 0.677652893618534
Lasso Train R2 Score: 0.5953854313600835
Ridge Train R2 Score: 0.6774318209283909

Linear Regression Test R2 Score: 0.6688554439500486
Lasso Test R2 Score: 0.6029339256174281
Ridge Test R2 Score: 0.6698172560614876

Linear Regression Coefficient: [ 2.73355403e-02, 2.03240535e+00, 3.77945513e+01, -2.73236122e+00, -3.15431235e-01, 4.35954671e-02]
Linear Regression Intercept: 14.710967559290044


 
**Random Forest Model Scores:**
We also used a Random Forest Model knowing that our dataset was on the lower end in quatity, to help add more variation and randomness to our data. This model predicted extremely well with an R2 score of 0.85 on our testing data.


Random Forest Score on Training (No GS): 0.9737978695026748
Random Forest Score on Testing (No GS): 0.8421494595338586

RFR Best Param: {'max_depth': 5, 'n_estimators': 100}
Random Forest GS Score on Training: 0.874002660264225
Random Forest GS Score on Testing: 0.8548869392466454


### Workflow Summary:
We programmed our algorithm to pull in the data that we retreived through our online partners' databases in the form of a csv file and turn it in to a dataframe that can allow for easy manipulation of data. This data frame was cleaned and explored for trends within the existing data and analyzed with predictive modeling to confirm or highlight the story that our data is telling us. We then evaluate the outputs of each model's to interpret what connections our chosen features had with our target variable, the Number of Games.

### Future Considerations:
Going forward, our team would like to explore different online filters when retreiving player statistics. We would also take more time to explore the data through a more extensive time frame. Given that the league is has only been around 24 years, that is very attainable. Lastly, Houston Analytics would further consider other options when feature engineering, especially a player's rookie year and the values that don't seem to have much correlation to the target variable. 