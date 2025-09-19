# Bike-price-prediction
# Overview
    This project predicts the selling price of used bikes using various features such as bike model, manufacture year, kilometers driven, seller type, and ownership.
    Two models are developed:
###   1. Model without ex_showroom_price  — Drops the ex_showroom_price column due to many missing values.
###   2. Model with imputed ex_showroom_price — Imputes missing showroom prices per bike model using median values to retain this informative feature.
# Dataset
    Contains 1,061 bike listings with columns: name, selling_price, year, seller_type, owner, km_driven, and ex_showroom_price.
    Missing ex_showroom_price values imputed based on median prices per bike model (in second model only).
# Model Performance
   Model	                       R²           	MAE              	RMSE
Without ex_showroom_price	      ~0.44         	~18,900         	~38,600
With imputed ex_showroom_price	~0.86         	~12,000          	~19,200
