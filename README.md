# <b>PRCP-1012
# <b>GAME WINNER PREDICTION

## <B>CONTRIBUTION 
    SHEKHAR KHAIRNAR


# <b>BUSINESS PROBLEM

## <b>PROBLEM CONTEXT
<b>
    
- BASED ON GIVEN FEATURE AND MESUREMENT PREDICT THE WIN PROBABILITY OF PUBG MATCH

  ## <b>REGRESSION TASK

  # <b>TASK 1
#### <b>PREPARE A COMPLETE DATA ANALYSIS REPORT ON THE GIVEN DATA.

# <b>TASK 2
#### <b>CREATE A PREDICTIVE MODEL WHICH IS AN ATTEMPT TO PREDICT THE WIN PROBABILITY OF THE PUBG MATCH AND TO LOOK AT THE IMPORTANT FACTORS AFFECTING THE WIN PROBABILITY OF THE PUBG GAME.


### <b>TYPES OF MACHINE LEARNING PROBLEM.
- <b>Regression is a supervised learning technique where the goal is to predict a continuous numerical value for each data point, based on labeled training data consisting of input features and their corresponding real-valued outputs.<br>
### <b>ALGORITHM USES FOR REGRESSION
<b>
    
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- XGBoost
- Gradient Boosting Regressor


## <b>DOMAIN ANALYSIS
<b>
TARGET COLUMN == winPlacePerc</b><br>

## <b>Features:

- <b>DBNOs</b><br>
Number of enemy players knocked.
- <b>assists</b><br>Number of enemy players this player damaged that were killed by teammates.
- <b>boosts</b><br>Number of boost items used.
- <b>damageDealt</b><br>Total damage dealt. Note: Self inflicted damage is subtracted.
- <b>headshotKills</b><br>Number of enemy players killed with headshots.
- <b>heals</b><br>Number of healing items used.
- <b>Id</b><br>Player’s Id
- <b>killPlace </b><br> Ranking in match of number of enemy players killed.
- <b>killPoints </b><br> Kills-based external ranking of player. (Think of this as an Elo ranking where only kills matter.) If there is a value other than -1 in - - rankPoints, then any 0 in killPoints should be treated as a “None”.
- <b>killStreaks </b><br> Max number of enemy players killed in a short amount of time.
- <b>kills </b><br> Number of enemy players killed.
- <b>longestKill </b><br> Longest distance between player and player killed at time of death. This may be misleading, as downing a player and driving away may - -lead to a large longestKill stat.
- <b>matchDuration </b><br> Duration of match in seconds.
- <b>matchId </b><br> ID to identify match. There are no matches that are in both the training and testing set.
- <b>matchType </b><br> String identifying the game mode that the data comes from. The standard modes are “solo”, “duo”, “squad”, “solo-fpp”, “duo-fpp”, and “squad-fpp”; other modes are from events or custom matches.
- <b>rankPoints </b><br> Elo-like ranking of player. This ranking is inconsistent and is being deprecated in the API’s next version, so use with caution. Value of -1 takes place of “None”.
- <b>revives </b><br> Number of times this player revived teammates.
- <b>rideDistance </b><br> Total distance traveled in vehicles measured in meters.
- <b>roadKills </b><br> Number of kills while in a vehicle.


## <b>TRAINING AND TESTING MODEL COMPARISON
| **Model**                       | **Train R² Score** | **Test R² Score** |
| ------------------------------- | ------------------ | ----------------- |
| **Linear Regression**           | 0.7788             | 0.7786            |
| **Decision Tree Regressor**     | 0.9999             | 0.8523            |
| **Random Forest Regressor**     | 0.9857             | 0.9198            |
| **XGBoost**                     | 0.9278             | 0.9264            |
| **Gradient Boosting Regressor** | 0.9064             | 0.9058            |


### <b>RESULT SUMMARY
<b>1) Linear Regression:</b>

    - Train R²: 0.779
    - Test R²: 0.779
    - The model performs fairly well, showing a good balance between training and testing performance, suggesting no significant overfitting.
<br>
<b>2) Decision Tree Regressor:</b>

    - Train R²: 0.99995
    - Test R²: 0.852
    - The model is highly overfit to the training data (near-perfect performance), but it still generalizes well to the test data, though with a notable drop.
<br>
<b>3) Random Forest Regressor:</b>

    - Train R²: 0.9857
    - Test R²: 0.9198
    - This model shows a very strong performance on both training and testing data, indicating good generalization with a small drop in performance on the test set.
<br>
<b>4) XGBoost:</b>

    - Train R²: 0.9278
    - Test R²: 0.9264
    - The XGBoost model is consistent, with almost no drop between training and test data, indicating it is robust and generalizes well.
<br>
<b>5) Gradient Boosting Regressor:</b>

    - Train R²: 0.9064
    - Test R²: 0.9058
    - Similar to XGBoost, this model shows strong consistency, with a small but acceptable drop in performance between training and test data.
<br>
<b>OBSERVATION</b>
    
- The Decision Tree Regressor shows overfitting, though it still performs decently on test data.
- Random Forest, XGBoost and Gradient Boosting all perform well with strong generalization capabilities.
- XGBoost and Gradient Boosting are quite robust, with little difference between training and test performance.

# <B>THANK YOU
# <b>END OF PROJECT
<b>SHEKHAR KHAIRNAR
