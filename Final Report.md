**2022 NCAA Probability Prediction**

*Authors: Muhab Elgamal, Rajvinder Singh, Christian Saliski*

**Abstract**

In this project, we tackle the challenge of predicting the win probabilities of teams participating in the NCAA March Madness tournament. Leveraging a variety of CSV files containing information about team performances in regular seasons and past tournaments, we aimed to develop a model that could forecast the outcome of matchups. We extracted data points like scores, field goal percentages, and blocks to train our model. Our approach involved data manipulation and merging to create a dataset suitable for training. The resulting predictions were saved in a CSV file, featuring team IDs, corresponding opponent IDs, and the win probability for each team against its opponent. Surprisingly, the predicted probabilities ranged from high chances of 85% to mere 5% chances, revealing intriguing insights into potential matchups.

**Introduction**

Predicting winners in the NCAA March Madness tournament is a challenging task due to the myriad factors influencing game outcomes. Our approach seeks to make predictions solely based on historical statistical data rather than considering factors like player injuries. This has significant implications for sports betting, as an accurate predictive model could offer substantial benefits to gamblers. We present our predictions in a CSV file containing win probabilities for various matchups, enabling users to quickly find the expected outcomes.

**Related Work**

Our project aligns with the broader theme of predicting NCAA tournament outcomes. While numerous betting platforms allow bracket predictions, our approach stands out by relying on historical data for training. However, this approach faces limitations due to its inability to account for present changes in team dynamics, like player injuries. Despite these challenges, our utilization of LightGBM, a gradient boosting model, combined with jax's mathematical accuracy, contributed to our competitive performance in the Kaggle competition.

**Data**

The project involved wrangling and merging data from multiple CSV files spanning several years. These files contained extensive game and team statistics, necessitating a rigorous data preparation process. Teams were linked using unique identifiers (TeamID), and this data was sourced from Kenneth Massey's database. Extensive pandas operations were employed to create a cohesive dataset for training.

**Methods**

Our methodology involved gathering and preprocessing data, training a predictive model, and generating win probabilities. We experimented with different models and landed on using LightGBM, a fast and efficient gradient boosting framework. Incorporating jax further enhanced our model's accuracy. Although our model's accuracy fell short due to unpredictable tournament upsets, our approach showcases the potential of such models for public applications.

**Experiments**

We conducted experiments to refine our model and find optimal training times. We observed fluctuations in probabilities as training times increased, but due to time constraints, we settled on 10-minute training intervals. The model's average win probability for each team was calculated and ranked to identify the most likely tournament winners.

**Conclusion**

Our project demonstrates the potential of data-driven approaches in predicting NCAA March Madness outcomes. While we learned the intricacies of manipulating CSV files and applying jax to enhance model accuracy, we also recognize the limitations of historical data in predicting tournament upsets. Future extensions could involve incorporating present-season data and player statistics to improve predictive power. Overall, our project offers insights into the potential of predictive models in sports betting and tournament analysis.
