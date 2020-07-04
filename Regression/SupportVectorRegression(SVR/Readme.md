About dataset: A small dataset containing the salaries according to different employee positions.

SVR aims to minimize coefficient instead of minimizing squared error. It uses epsilon-insensitive tube. The values inside this tube are considered as within-range, that means SVR can be used when we want flexibility in our model to define how much error is acceptable in our model.
Slack vairables determine the values outside of epsilon tube.

We will need to do feature scaling because unlike MLR, we don't have a coefficient to balance out the effect of large values.

