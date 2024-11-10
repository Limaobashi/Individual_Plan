# Individual_Plan

1. Data Description
 
 (1) players.csv
 
There are 197 observations and 9 variables in this dataset, among them, there are seven columns with detailed data: experience, subscribe, hashedEmail, played_hours, name, gender, and age. Among them, experience is divided into five types: Pro, Veteran, Amateur, Regular, and Beginner, which represent each observation’s familiarity with the game. Subscribe indicates whether the player has registered for the game, with two categories: TRUE or FALSE. The third column is their email, with this variable being of text type. Played_hours refers to the time they’ve spent playing the game, a numeric type, while the remaining two columns display the player’s gender and age. From this chart, we can observe that players who haven’t registered for the game have 0 game time, though some registered players also have 0 game time. Participants include both males and females, with most ages clustered around 20. Game time varies widely among players, with the highest reaching 223 hours. However, I cannot directly determine the relationship between game time and other variables, so we can use data visualization to explore potential correlations. In the next phase of the project, we can use these variables to predict players' game time and observe which types of players tend to play longer.

 (2)sessions.csv

 There are 1536 observations and 5 variables in this dataset which includes hashedEmail, the time that players start and end the game. Besides, there are also original strat and end time. Acturally, we can ignore the last two variables.



 2. Question

 Our group focus on the first question: We would like to know which "kinds" of players are most likely to contribute a large amount of data so that we can target those players in our recruiting efforts. In "players.csv" file, we are interested in the played_hour, that is the instrest. And we can use experience, gender and age to predict what types of play could play it for a long time and contribute a large amount of data. We can use experience, gender and age as predictors, and trian model to chose a suitable model in order to get accurate prediction results.



3. Exploratory Data Analysis and Visualization



4. Methods and Plan

I think we can use k-nn regression or linear regression to address our question. There are enough data to set training data and testing data to choose an apporiate "K" and test the accuracy of this way to choose a best model. However, it also have some limitations, if we have more variables to predict the results and have more observations to train the model, it will be better, we need more data. As for choose the model, we can calculate the RMSPE of models to choose the accuratest one which has the smallest RMSPE. When we choose the model in k-nn regression and linear regression, we need split the data into testing part and training part, among them, training data make up 70%. And we also need to use cross validation to choose a best "K" in k-nn regression.
