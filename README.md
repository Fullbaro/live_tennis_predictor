# The idea

In this data analysis project, I aim to predict the outcomes of tennis matches by leveraging live match data. Unlike traditional approaches that utilize various game statistics, my innovative approach revolves around strategically reversing the role of bookmakers. I employ real-time odds for individual players as a primary predictor to determine the ultimate winner while the match is in progress. While additional parameters contribute to the predictive model, the central element lies in utilizing odds provided by bookmakers. This novel methodology seeks to capitalize on the unique insights offered by betting markets to enhance the accuracy of match outcome predictions.

**Each match is treated as a time series, so the prediction is not just based on a specific time, but every event since the start of the match is used in the decision**

There's a saying that you can only create something new if there is no data set that matches your idea. I couldn't find the right data set for me, so I spent a couple of weeks gathering data on my own in a separate project. After the analyses were done, and after training several models in a separate project, a web interface was created where live predictions for the current matches are available. This is still under development and not publicly available

<p align="center">
  <img src="https://raw.githubusercontent.com/Fullbaro/live_tennis_predictor/main/assets/img.png" width="500" title="screenshot">
</p>

# The notebook speaks for itself, you can see it [HERE](https://github.com/Fullbaro/live_tennis_predictor/blob/main/main.ipynb)

# Results
Testing in a live environment showed that the model can successfully predict the winner during the match. Unfortunately, it is not suitable for sports betting purposes, because when the level of confidence in some decisions reaches an acceptable level, even the bookmakers give very low odds on the outcome. The model tracks changes in odds too closely.

