# Machine learning

### Description
We use a synthetic dataset `house_prediction_dataset.csv`containing 10,000 samples of residential property data, generated to simulate real-world housing market behavior.
Each row represents a single house and includes a mix of structural and locational features commonly used in regression-based price prediction models — such as `square_feet`, `number of rooms`, `age`, and `distance from the city(km)`.
The target price variable is derived from these inputs using a realistic linear combination with added noise, where we want to experiment with `LinearRegression` and `RandomForestRegressor`.
So we ask ourselves: can we predict the price of accommodation? 

### How to run? 

1. Create environment in conda `conda create --name house_price_prediction python=3.10`
2. Activate that environment `conda activate house_price_prediction`
3. Install requirement file `pip install -r requirements.txt`
4. Install ipykernel `python -m ipykernel install --user --name=house_price_prediction`
5. Open notebook in jupyter and select `house_price_prediction` as pykernel


### Conclusion
- By using all features instead of only selected few, we reduced RMSE from 18% to 7%.
- The proportion of variance in the dependent variable that is predictable from the independent variables R2 has increased from 75% to 95%.
- Our hypothesis that by separating negative prices, the result should be better did not turn out to be correct.
- In our case, LinearRegression (7%) shows better results than RandomForestRegressor (9%).
- This data set clearly shows that each feature affects the price and should not be separated as such.






-----
#### Team Members:
- Madeleine Thunholm
- Ali Asheer
- Adrian Kaczor
- Ivana Lovric