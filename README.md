# Neural-Network-Stock-Market-Trading-Algorithm
This project was a group effort between myself, Ting-Jung Lee, and Alan Bohnert as our Final Project 
for MATH 5399 Advanced Problems: Machine Learning with Python (Summer 2023 term) taught by Dr. Monico.

In our analysis, we attempted to predict a future day’s stock returns in the form of that day’s 
log(return). We assigned the predicted day’s log(return) to one of four categories based on the 
magnitude of the potential loss or gain of the log(return): 0 being a major loss, 1 being a minor 
loss, 2 is a minor return, and 3 is a major return. To predict the next day’s log(returns), we 
constructed three models with different input data from the previous three days. First, we used 
three consecutive days of log(returns) to predict the subsequent day’s log(return). Based on our 
neural network model we found the accuracy of our model to be approximately 31%, which was a 
statistically significant finding according to our hypothesis test using a confidence level of 99%. 
The second model uses three consecutive days’ trade volumes divided by a 60-day rolling mean 
volume to predict the log(return) of the subsequent day. Intuitively, volume alone should not be 
able to predict returns, and our model bears this out with an accuracy of roughly 25% which is not 
statistically better than choosing randomly. Finally, we used three consecutive days of log(returns) 
and the corresponding three scaled volumes for those same days to determine the subsequent day’s 
log(return) category. Using all of this information, our model returned approximately 29% and is 
a statistically significant finding according to our hypothesis test. 
