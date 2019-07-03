Second Order Cone Programming (SOCP) functionality was released at Mark 27 of the NAG library

## Portfolio Optimisation using Second Order Cone Programming (SOCP)

A walk-through of modelling techniques in portfolio optimization using second-order cone programming in the NAG Library. Models in portfolio optimization include

* quadratic programming (efficient frontier)
* quadratically constrained quadratic programming (tev portfolio)
* optimization with objective of fraction of quadratic and linear (the Sharpe ratio).

General functions are enclosed for users to get the principle idea on SOCP reformulation. They provide one of the ways to build and solve their problems using NAG's SOCP solver and could be copy and paste into a model and reuse repeatedly.               

* [portfolio_optimisation_using_socp.ipynb](./portfolio_optimisation_using_socp.ipynb) - Jupyter notebook
* [portfolio_optimisation_using_socp.pdf](./static/portfolio_optimisation_using_socp.pdf) - Static pdf version
* [portfolio_optimisation_using_socp.html](./static/portfolio_optimisation_using_socp.html) - Static html version


# Files included here 

stock_price.pkl - pickled data file contains daily prices of 30 stocks in
                  DJIA from March 2018 to March 2019. It is used to estimate
                  out-of-sample expected return and covariance matrix.


### Building the pdf version

The notebook uses the `latex_envs` Jupyter extension at https://jupyter-contrib-nbextensions.readthedocs.io/en/latest/nbextensions/latex_envs/README.html and attempting to produce the pdf version from the Jupyter GUI did not work. Instead, The pdf output was produced from the notebook using the following command after the `latex_envs` extension was installed.

```
jupyter nbconvert --to pdf portfolio_optimisation_using_socp.ipynb
```

