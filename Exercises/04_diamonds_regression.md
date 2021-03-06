Exercise - Regression on the diamonds data set
================

You will find an Artifical Neural Network implemented in keras capable
of predicting the price of a diamond here:
[R/04\_diamonds\_regression.R](https://github.com/leonjessen/RPharma2019/blob/master/R/04_diamonds_regression.R)
(This script is also in the directory `/R` of your RStudio session)

*Your task is to, make the script run and find and tune the
hyperparameters to get a working model*

The model is working, when the `Actual Price of Diamond` is equal to the
`Predicted Price of Diamond` in the final plot. (`y_pred` values are
equal to the `y_true`, look for the dashed identity line).

<details>

<summary>When you have the script running and a working model, click
here to see suggested hyperparameters</summary>

``` r
n_epochs      = 50
batch_size    = 50
loss          = 'mean_squared_error'
learning_rate = 0.001
optimzer      = optimizer_adam(lr = learning_rate)
h1_activation = 'relu'
h1_n_hidden   = 9
h2_activation = 'relu'
h2_n_hidden   = 9
h3_activation = 'relu'
h3_n_hidden   = 9
o_activation  = 'linear'
```

Try to use this as a reference and then increase of decrease the model
complexicity to see if you can find an even better architecture.

</details>
