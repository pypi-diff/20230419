# Comparing `tmp/predict_eth-0.1.1.tar.gz` & `tmp/predict_eth-0.1.2.tar.gz`

## Comparing `predict_eth-0.1.1.tar` & `predict_eth-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 predict_eth-0.1.1/developers.md
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 predict_eth-0.1.1/release-process.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 predict_eth-0.1.1/requirements.txt
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 predict_eth-0.1.1/challenges/hack1.md
--rw-r--r--   0        0        0     6656 2020-02-02 00:00:00.000000 predict_eth-0.1.1/challenges/main1.md
--rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 predict_eth-0.1.1/challenges/main2.md
--rw-r--r--   0        0        0     9274 2020-02-02 00:00:00.000000 predict_eth-0.1.1/challenges/main3.md
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 predict_eth-0.1.1/examples/.DS_Store
--rw-r--r--   0        0        0     7199 2020-02-02 00:00:00.000000 predict_eth-0.1.1/examples/end-to-end_compare-models.md
--rw-r--r--   0        0        0     5625 2020-02-02 00:00:00.000000 predict_eth-0.1.1/examples/end-to-end_optimized.md
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 predict_eth-0.1.1/examples/end-to-end_simple.md
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 predict_eth-0.1.1/examples/get-ethdata-binance-direct.md
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 predict_eth-0.1.1/examples/get-ethdata-ccxt-binance.md
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 predict_eth-0.1.1/examples/get-ethdata-ocean-binance.md
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 predict_eth-0.1.1/examples/get-ethdata-ocean-thegraph.md
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 predict_eth-0.1.1/ideas/.DS_Store
--rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 predict_eth-0.1.1/ideas/algorithmic-trading-flow.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 predict_eth-0.1.1/ideas/articles.md
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 predict_eth-0.1.1/ideas/data-sources.md
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 predict_eth-0.1.1/ideas/modeling.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predict_eth-0.1.1/predict_eth/__init__.py
--rw-r--r--   0        0        0     4726 2020-02-02 00:00:00.000000 predict_eth-0.1.1/predict_eth/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predict_eth-0.1.1/predict_eth/test/__init__.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 predict_eth-0.1.1/predict_eth/test/test_helpers.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 predict_eth-0.1.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 predict_eth-0.1.1/LICENSE
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 predict_eth-0.1.1/README.md
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 predict_eth-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 predict_eth-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 predict_eth-0.1.2/developers.md
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 predict_eth-0.1.2/release-process.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 predict_eth-0.1.2/requirements.txt
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 predict_eth-0.1.2/challenges/hack1.md
+-rw-r--r--   0        0        0     6640 2020-02-02 00:00:00.000000 predict_eth-0.1.2/challenges/main1.md
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 predict_eth-0.1.2/challenges/main2.md
+-rw-r--r--   0        0        0     9049 2020-02-02 00:00:00.000000 predict_eth-0.1.2/challenges/main3.md
+-rw-r--r--   0        0        0    10627 2020-02-02 00:00:00.000000 predict_eth-0.1.2/challenges/main4.md
+-rw-r--r--   0        0        0    10640 2020-02-02 00:00:00.000000 predict_eth-0.1.2/challenges/main5.md
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 predict_eth-0.1.2/examples/.DS_Store
+-rw-r--r--   0        0        0     7235 2020-02-02 00:00:00.000000 predict_eth-0.1.2/examples/end-to-end_compare-models.md
+-rw-r--r--   0        0        0     5446 2020-02-02 00:00:00.000000 predict_eth-0.1.2/examples/end-to-end_optimized.md
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 predict_eth-0.1.2/examples/end-to-end_simple.md
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 predict_eth-0.1.2/examples/get-ethdata-binance-direct.md
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 predict_eth-0.1.2/examples/get-ethdata-ccxt-binance.md
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 predict_eth-0.1.2/examples/get-ethdata-ocean-binance.md
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 predict_eth-0.1.2/examples/get-ethdata-ocean-thegraph.md
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 predict_eth-0.1.2/ideas/.DS_Store
+-rw-r--r--   0        0        0     9151 2020-02-02 00:00:00.000000 predict_eth-0.1.2/ideas/algorithmic-trading-flow.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 predict_eth-0.1.2/ideas/articles.md
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 predict_eth-0.1.2/ideas/data-sources.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 predict_eth-0.1.2/ideas/modeling.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predict_eth-0.1.2/predict_eth/__init__.py
+-rw-r--r--   0        0        0     5126 2020-02-02 00:00:00.000000 predict_eth-0.1.2/predict_eth/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 predict_eth-0.1.2/predict_eth/test/__init__.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 predict_eth-0.1.2/predict_eth/test/test_helpers.py
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 predict_eth-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 predict_eth-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 predict_eth-0.1.2/README.md
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 predict_eth-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4847 2020-02-02 00:00:00.000000 predict_eth-0.1.2/PKG-INFO
```

### Comparing `predict_eth-0.1.1/developers.md` & `predict_eth-0.1.2/developers.md`

 * *Files identical despite different names*

### Comparing `predict_eth-0.1.1/release-process.md` & `predict_eth-0.1.2/release-process.md`

 * *Files identical despite different names*

### Comparing `predict_eth-0.1.1/challenges/hack1.md` & `predict_eth-0.1.2/challenges/hack1.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!--
-Copyright 2022 Ocean Protocol Foundation
+Copyright 2023 Ocean Protocol Foundation
 SPDX-License-Identifier: Apache-2.0
 -->
 
 # Quickstart: Predict Future ETH Price: For Web3 ATL Hackathon
 
 This quickstart describes a flow to predict future ETH price via a local AI model.
```

### Comparing `predict_eth-0.1.1/challenges/main1.md` & `predict_eth-0.1.2/challenges/main1.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 <!--
-Copyright 2022 Ocean Protocol Foundation
+Copyright 2023 Ocean Protocol Foundation
 SPDX-License-Identifier: Apache-2.0
 -->
 
-# Quickstart: Predict Future ETH Price
+# Predict-ETH Round 1
 
 This quickstart describes a flow to predict future ETH price via a local AI model.
 
-It is used for the first [ETH Prediction Challenge](https://blog.oceanprotocol.com/ocean-protocol-announces-the-launch-of-the-eth-prediction-challenge-7b1f04cc820e)
+It is used for [Predict-ETH Round 1 Data Challenge](https://blog.oceanprotocol.com/ocean-protocol-announces-the-launch-of-the-eth-prediction-challenge-7b1f04cc820e)
 
 - Kickoff: Oct 2, 2022
 - Submission deadline: Oct 16, 2022 at 23:59 UTC
 - Prediction at times: Oct 17, 2022 at 1:00 UTC, 2:00 UTC, ..., 23:00, 24:00. (24 predictions total). 
 - Winners announced: within one week
 
 Here are the steps:
@@ -218,8 +218,8 @@
 
 cex_vals = filter_to_target_uts(target_uts, allcex_uts, allcex_vals)
 
 #calc nmse, plot
 nmse = calc_nmse(cex_vals, pred_vals)
 print(f"NMSE = {nmse}")
 plot_prices(cex_vals, pred_vals)
-```
+```
```

### Comparing `predict_eth-0.1.1/challenges/main2.md` & `predict_eth-0.1.2/challenges/main2.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!--
-Copyright 2022 Ocean Protocol Foundation
+Copyright 2023 Ocean Protocol Foundation
 SPDX-License-Identifier: Apache-2.0
 -->
 
-# Predict ETH Price: Round Two 
+# Predict-ETH Round 2
 
-This is the main readme for the [Ocean Data Challenge :: ETH Prediction Round 2](https://questbook.app/explore_grants/about_grant/?grantId=0x9f248741962aaf27bd10f2c50aeec2d13f343611&chainId=137). 
+This is the main readme for the [Predict-ETH Round 2 Data Challenge](https://questbook.app/explore_grants/about_grant/?grantId=0x9f248741962aaf27bd10f2c50aeec2d13f343611&chainId=137). 
 
 - Kickoff: Nov 14, 2022
 - Submission deadline: Dec 11, 2022 at 23:59 UTC
 - Prediction at times: Dec 12, 2022 at 1:00 UTC, 2:00, ..., 12:00 (12 predictions total).
 - Winners announced: within one week
 - To be considered for winning, and for 250 OCEAN reward for a valid submission, prediction error must (a) lower than if the "prediction" was simply a constant (b) lower than any of the end-to-end examples' prediction errors
```

### Comparing `predict_eth-0.1.1/challenges/main3.md` & `predict_eth-0.1.2/challenges/main3.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 <!--
-Copyright 2022 Ocean Protocol Foundation
+Copyright 2023 Ocean Protocol Foundation
 SPDX-License-Identifier: Apache-2.0
 -->
 
-# Predict ETH Price: Round Three
+# Predict-ETH Round 3
 
 ## 0. Introduction
 
-This is the main readme for the Ocean Data Challenge :: ETH Prediction Round 3.
+This is the main readme for Predict-ETH Round 3 Data Challenge.
 
 ### 0.1 Key dates
 
 - Kickoff: Jan 16, 2023
 - Submission deadline: Sun Feb 19, 2023 at 23:59 UTC
 - Prediction at times: Mon Feb 20, 2023 at 1:00 UTC, 2:00, ..., 12:00 (12 predictions total).
-- Winners announced: within one week. See previous challenge results [here]( https://blog.oceanprotocol.com/introducing-the-winners-of-the-eth-price-prediction-data-challenge-edition-2-6acdccb9271)
 
 ### 0.2 Criteria to win
 - Weighting:
   - 50% - lowest prediction error
   - 25% - presentation of approach, and feedback
   - 25% - proper flow was used to submit. This includes: the predictions were stored to arweave, and a datatoken was shared to judges. (This README covers how to do both.)
 - To be considered for winning, prediction error must lower than if the "prediction" was simply a constant.
```

### Comparing `predict_eth-0.1.1/examples/.DS_Store` & `predict_eth-0.1.2/examples/.DS_Store`

 * *Files identical despite different names*

### Comparing `predict_eth-0.1.1/examples/end-to-end_compare-models.md` & `predict_eth-0.1.2/examples/end-to-end_compare-models.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 In this README, each model uses the previous 12 hours' of prices to predict the next 12 hours' worth.  
 
 Four modeling approaches are used: Linear Regression, Random Forests, Support Vector Machine, and a two-layer densely-connected neural nework.
 
 ## 1. Setup
 
-We assume you've already done [main3.md](../challenges/main3.md#1-setup) "Setup".
+We assume you've already done [main5.md](../challenges/main5.md#1-setup) "Setup".
 
 Let's install TensorFlow. We do it here, and not earlier, because it's 500MB. In the console:
 
 ```console
 pip3 install tensorflow
 ```
 
@@ -27,15 +27,15 @@
 
 ```python
 import ccxt
 import pandas as pd
 import numpy as np
 import requests
 
-cex_x = ccxt.binance().fetch_ohlcv('ETH/USDT', '1h')
+cex_x = ccxt.binance().fetch_ohlcv('ETH/USDT', '5m')
 
 # create a Data Frame with two columns [date,eth-prices] with dates given in intervals of 1-hour
 import pandas as pd
 data = pd.DataFrame(cex_x, columns=['date', 'open', 'max', 'min', 'close', 'volume'])
 data['date'] = pd.to_datetime(data['date'],unit='ms')
 
 # Divide the data in training and testing set. Because the data has temporal structure, we split the data in two blocks, vs. selecting randomly.
@@ -132,45 +132,45 @@
 fig = plt.figure(figsize = (10, 5))
  
 # creating the bar plot
 plt.bar(methods, values, color ='maroon', width = 0.4)
  
 plt.xlabel("Methods")
 plt.ylabel("NMSE")
-plt.title("Comparison of different methods for predicting ETH value 1-12 hours ahead")
+plt.title("Comparison of different methods for predicting ETH value 1-12 time periods ahead")
 plt.show()
 ```
 
-### 3.2 Run the AI model to make future ETH price predictions"
+### 3.2 Run the AI model to make future ETH price predictions
 
 #### 3.2.1 Select the best performant model and make final predictions
 
 Looking at the averaged error on the test set, we observe that the Random Forest Regression provides the lowest NMSE.The ranking of the methods will change depending on the hyper parameters selected and in the case of Neural Networks, initialization is critical. With the RFR selected, we proceed to retrain the model using all the available data up to the current time.
 
 In the same Python Console:
 
 ```python
 full_data_close = pd.concat([data['close'].shift(i) for i in range(0,max_lag)],axis=1).dropna().values
 full_data_open = pd.concat([data['open'].shift(i) for i in range(0,max_lag)],axis=1).dropna().values
 Y = full_data_close[max_lag:,:]
 X = np.concatenate((full_data_close[0:-max_lag,:],full_data_open[0:-max_lag,:]),axis=1)
 model = RegressorChain(base_estimator=rfr).fit(X, Y)  
 ```
-Then we create the prediction for the future values 1h, 2h, ... 12h. For this example, the input is the feature vector corresponding to the latest observed data point:
+Then we create the prediction for the future values 5min, 10min, ... 60min. For this example, the input is the feature vector corresponding to the latest observed data point:
 
 ```python
-# predict future 12 hours prices using latest 12 values observed
+# predict future 12 time periods prices using latest 12 values observed
 input_data = np.concatenate((full_data_close[-1:,:],full_data_open[-1:,:]),axis=1)
 pred_vals = model.predict(input_data)
 ```
 
 ### 3.3 Calculate NMSE
 
 The NMSE was already calculated in section 3.1. The Random Forest had the lowest error.
 
-## 4.  Publish predictions
-From [Challenge 3](../challenges/main3.md), do:
-- [x] Publish predictions
+## 4.  Publish & share predictions
+From [Challenge 5](../challenges/main5.md), do:
+- [x] Publish & share predictions
 
 ## 5. Discussion
 
 There are many ways to reduce error further, including: more data, tuning hyperparameters, better feature vectors, better modeling algorithms including time-aware ones (e.g. recurrent neural networks).
```

### Comparing `predict_eth-0.1.1/examples/end-to-end_optimized.md` & `predict_eth-0.1.2/examples/end-to-end_optimized.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 <!--
-Copyright 2022 Ocean Protocol Foundation
+Copyright 2023 Ocean Protocol Foundation
 SPDX-License-Identifier: Apache-2.0
 -->
 
 # Simple End-to-end Example
 
 ## 0. Introduction
 
 This example predicts future ETH price, using simple input data (just historical ETH price) and a simple model (linear dynamical model).
 
-Predictions are 1h, 2h, ..., 12h into the future.
+Predictions are 5m, 10m, ..., 60m into the future.
 
 ## 1. Setup
 
-We assume you've already done [main3.md](../challenges/main3.md#1-setup) "Setup".
-
-If needed, re-setup in Python:
-- Do ocean.py [setup-remote.md](https://github.com/oceanprotocol/ocean.py/blob/main/READMEs/setup-remote.md#6-setup-in-python) "Setup in Python"
-- And do: `from predict_eth.helpers import *`
-
+We assume you've already done [main5.md](../challenges/main4.md#1-setup) "Setup".
 
 ## 2. Get data locally
 
 In the Python console:
 
 ```python
 import ccxt
-cex_x = ccxt.binance().fetch_ohlcv('ETH/USDT', '1h')
+cex_x = ccxt.binance().fetch_ohlcv('ETH/USDT', '5m')
 allcex_uts = [xi[0]/1000 for xi in cex_x] # timestamps
 allcex_vals = [xi[4] for xi in cex_x] # ETH prices
 
 # Extracts dates and ether price values
 print_datetime_info("CEX data info", allcex_uts)
 
 # Transform timestamps to dates
@@ -44,15 +39,15 @@
 ## 3.  Make predictions
 
 ### 3.1  Build an AI model
 
 In the same Python console:
 
 ```python continuation
-# use the last 12 hours of testing set, all the previous data is used as training
+# use the last 12 time periods of 5mins each of testing set, all the previous data is used as training
 train_data = data.iloc[0:-12,:]
 test_data = data.iloc[-12:,:]
 
 # fit a linear model (Open sourced Facebook's Prophet model: https://facebook.github.io/prophet/)
 # As the data is subdaily, the model will fit daily seasonality
 from prophet import Prophet
 model = Prophet()
@@ -104,17 +99,17 @@
 ```
 
 #### 3.4.2 Generate cross-validation parameters
 
 If you are wondering what these parameters are and/or what cross-validation mean, [here](https://blog.oceanprotocol.com/capitalize-with-ocean-protocol-a-predict-eth-tutorial-b2da136633f0) you can find a brief introduction to what Prophet does under the hood.
 ```python continuation
 # Set parameters for doing cross-validation
-horizon = "12 hours"
-initial = "15 days"
-period = "12 hours"
+horizon = "1 hours"
+initial = "1 days"
+period = "1 hours"
 ```
 
 #### 3.4.3 Generate hyperparameters combination
 ```python continuation
 # Generate grid for hyperparameters
 param_grid = {  
     "changepoint_prior_scale": [0.001, 0.01, 0.1, 0.5],
@@ -169,20 +164,20 @@
 
 ```python continuation
 # fit model with all the available data
 
 model = Prophet(**best_params) # Change to Prophet() if 3.4 skipped
 model.fit(data)
 
-# generate dates for prediction (12 hours ahead of the latest datapoint in the data time)
-future_dates = model.make_future_dataframe(periods=12, freq="h", include_history=False)
+# generate dates for prediction (12 time periods ahead of the latest datapoint in the data time)
+future_dates = model.make_future_dataframe(periods=12, freq="5min", include_history=False)
 
 # predcit eth values on future_dates
 forecast = model.predict(future_dates)
 pred_vals = forecast.set_index('ds')['yhat'].to_numpy()
 
 ```
 
 
-## 4.  Publish predictions
-From [Challenge 3](../challenges/main3.md), do:
-- [x] Publish predictions
+## 4.  Publish & share predictions
+From [Challenge 5](../challenges/main5.md), do:
+- [x] Publish & share predictions
```

### Comparing `predict_eth-0.1.1/examples/end-to-end_simple.md` & `predict_eth-0.1.2/examples/end-to-end_simple.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,59 +1,55 @@
 <!--
-Copyright 2022 Ocean Protocol Foundation
+Copyright 2023 Ocean Protocol Foundation
 SPDX-License-Identifier: Apache-2.0
 -->
 
 # Simple End-to-end Example
 
 ## 0. Introduction
 
 This example predicts future ETH price, using simple input data (just historical ETH price) and a simple model (linear dynamical model).
 
-Predictions are 1h, 2h, ..., 12h into the future.
+Predictions are 5mins, 10mins, ..., 60mins into the future.
 
 ## 1. Setup
 
-We assume you've already done [main3.md](../challenges/main3.md#1-setup) "Setup".
-
-If needed, re-setup in Python:
-- Do ocean.py [setup-remote.md](https://github.com/oceanprotocol/ocean.py/blob/main/READMEs/setup-remote.md#6-setup-in-python) "Setup in Python"
-- And do: `from predict_eth.helpers import *`
+We assume you've already done [main5.md](../challenges/main5.md#1-setup) "Setup".
 
 
 ## 2. Get data locally
 
 In the Python console:
 
 ```python
 
 import ccxt
-cex_x = ccxt.binance().fetch_ohlcv('ETH/USDT', '1h')
+cex_x = ccxt.binance().fetch_ohlcv('ETH/USDT', '5m')
 allcex_uts = [xi[0]/1000 for xi in cex_x] # timestamps
 allcex_vals = [xi[4] for xi in cex_x] # ETH prices
 
 # # Extracts dates and ether price values
 print_datetime_info("CEX data info", allcex_uts)
 
 # Transform timestamps to dates
 dts = to_datetimes(allcex_uts)
 
-# create a Data Frame with two columns [date,eth-prices] with dates given in intervals of 1-hour
+# create a Data Frame with two columns [date,eth-prices] with dates given in intervals of 5-minutes
 import pandas as pd
 data = pd.DataFrame({"ds": dts, "y": allcex_vals})
 ```
 
 ## 3.  Make predictions
 
 ### 3.1  Build an AI model
 
 In the same Python console:
 
 ```python
-# use the last 12 hours of testing set, all the previous data is used as training
+# use the last 12 intervals of 5mins each of testing set, all the previous data is used as training
 train_data = data.iloc[0:-12,:]
 test_data = data.iloc[-12:,:]
 
 # fit a linear model (Open sourced Facebook's Prophet model: https://facebook.github.io/prophet/)
 # As the data is subdaily, the model will fit daily seasonality
 from prophet import Prophet
 model = Prophet()
@@ -85,20 +81,20 @@
 Keep iterating in step 3 until you're satisfied with accuracy. Then...
 
 ```python
 # fit model with all the available data
 model = Prophet()
 model.fit(data)
 
-# generate dates for prediction (12 hours ahead of the latest datapoint in the data time)
-future_dates = model.make_future_dataframe(periods=12, freq="h", include_history=False)
+# generate dates for prediction (12 time perods ahead of the latest datapoint in the data time)
+future_dates = model.make_future_dataframe(periods=12, freq="5min", include_history=False)
 
 # predcit eth values on future_dates
 forecast = model.predict(future_dates)
 pred_vals = forecast.set_index('ds')['yhat'].to_numpy()
 
 ```
 
 
-## 4.  Publish predictions
-From [Challenge 3](../challenges/main3.md), do:
-- [x] Publish predictions
+## 4.  Publish & share predictions
+From [Challenge 5](../challenges/main5.md), do:
+- [x] Publish & share predictions
```

### Comparing `predict_eth-0.1.1/examples/get-ethdata-binance-direct.md` & `predict_eth-0.1.2/examples/get-ethdata-binance-direct.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 Here, we directly query the Binance API "Kline/Candlestick Data". [Here's the docs](https://binance-docs.github.io/apidocs/spot/en/#kline-candlestick-data). 
 
 We use Python [requests](https://requests.readthedocs.io/en/latest/) library to make queries.
 
 ### 0. Setup
 
-We assume you've already done [main3.md](../challenges/main3.md#1-setup) "Setup".
+We assume you've already done [main5.md](../challenges/main3.md#1-setup) "Setup".
 
 If needed, re-setup in Python:
 - Do ocean.py [setup-remote.md](https://github.com/oceanprotocol/ocean.py/blob/main/READMEs/setup-remote.md#6-setup-in-python) "Setup in Python"
 - And do: `from predict_eth.helpers import *`
 
 ### 1. Get Data
 
 In the Python console:
 ```python
 import requests
-url = f"https://api.binance.com/api/v3/klines?symbol=ETHUSDT&interval=1h"
+url = f"https://api.binance.com/api/v3/klines?symbol=ETHUSDT&interval=5m"
 r = requests.get(url)
 cex_x = r.json()
 
 # cex_x is a list 500 items, one for every hour, on the hour. 
 #
 # Each item has a list of 12 entries: 
 # (0) timestamp (1) open price (2) high price (3) low price (4) close price (5) Vol ..
```

### Comparing `predict_eth-0.1.1/examples/get-ethdata-ccxt-binance.md` & `predict_eth-0.1.2/examples/get-ethdata-ccxt-binance.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 Here, we use the the ccxt library, "a collection of available crypto exchanges or exchange classes. Each class implements the public and private API for a particular crypto exchange." [Here are ccxt docs](https://docs.ccxt.com/en/latest/manual.html). [Here's ccxt on github](https://github.com/ccxt/ccxt).
 
 Under the hood, ccxt queries the Binance API for Binance data.
 
 
 ### 0. Setup
 
-We assume you've already done [main3.md](../challenges/main3.md#1-setup) "Setup".
+We assume you've already done [main5.md](../challenges/main3.md#1-setup) "Setup".
 
 If needed, re-setup in Python:
 - Do ocean.py [setup-remote.md](https://github.com/oceanprotocol/ocean.py/blob/main/READMEs/setup-remote.md#6-setup-in-python) "Setup in Python"
 - And do: `from predict_eth.helpers import *`
 
 ### 1. Get Data
  
 In the Python console:
 
 ```python
 import ccxt
-cex_x = ccxt.binance().fetch_ohlcv('ETH/USDT', '1h')
+cex_x = ccxt.binance().fetch_ohlcv('ETH/USDT', '5m')
 
 # cex_x is a list of 500 items, one for every hour, on the hour.
 #
 # Each item has a list of 6 entries:
 # (0) timestamp (1) open price (2) high price (3) low price (4) close price (5) volume
 # Example item: [1662998400000, 1706.38, 1717.87, 1693, 1713.56, 2186632.9224]
 # Timestamp is unix time, but in ms. To get unix time (in s), divide by 1000
```

### Comparing `predict_eth-0.1.1/examples/get-ethdata-ocean-binance.md` & `predict_eth-0.1.2/examples/get-ethdata-ocean-binance.md`

 * *Files identical despite different names*

### Comparing `predict_eth-0.1.1/examples/get-ethdata-ocean-thegraph.md` & `predict_eth-0.1.2/examples/get-ethdata-ocean-thegraph.md`

 * *Files identical despite different names*

### Comparing `predict_eth-0.1.1/ideas/.DS_Store` & `predict_eth-0.1.2/ideas/.DS_Store`

 * *Files identical despite different names*

### Comparing `predict_eth-0.1.1/ideas/algorithmic-trading-flow.md` & `predict_eth-0.1.2/ideas/algorithmic-trading-flow.md`

 * *Files identical despite different names*

### Comparing `predict_eth-0.1.1/ideas/articles.md` & `predict_eth-0.1.2/ideas/articles.md`

 * *Files identical despite different names*

### Comparing `predict_eth-0.1.1/ideas/data-sources.md` & `predict_eth-0.1.2/ideas/data-sources.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 ## Data Sources
 
 Existing and potential future data sources to consider
 
 ### Already in one or more READMEs
 
 - data in Ocean Market
-- ccxt library - data from > 40 exchanges
+- ccxt library: Binance, ETH, close data
 - binance API
 
 ### Other potential data
-- Request data from Ethereum and Polygon from Transpose(https://docs.transpose.io/sql/getting-started/)
-- Pull data from Flipside, Footprint, Dune, Luabase, Google and BigQuery (large free data providers). Example: https://colab.research.google.com/drive/1zsxX28_vZMVLSSJYOLI5hv2zsdKH34T0?usp=sharing&authuser=1
+- ccxt library: other exchanges (40 supported), other coins (BTC, etc), more than close data (eg open, high, low, volume)
+- [Transpose](https://docs.transpose.io/sql/getting-started/) for data from Ethereum and Polygon 
+- [Dune Analytics](https://dune.com/browse/dashboards)
+- [Defi Lllama](https://defillama.com)
+- [Flipside Crypto](https://flipsidecrypto.xyz/)
+- [Uniswap.info](https://info.uniswap.org/)
+- [Example](https://colab.research.google.com/drive/1zsxX28_vZMVLSSJYOLI5hv2zsdKH34T0?usp=sharing&authuser=1) pulling data from Flipside, Footprint, Dune, Luabase, Google and BigQuery
 - [TrueBlocks data](https://trueblocks.io/data-model/intro/). All on-chain data [here](https://trueblocks.io/data-model/chaindata/)
 - [Messari subgraphs](https://github.com/messari/subgraphs). Status of all subgraphs [here](https://subgraphs.messari.io/) 
-- Web3 Data SQL Companies-Transpose, Flipside Crypto, Dune Analytics - Transpose most open to integration, SQL for datasets->train model 
-- Ocean Missions-OceanDAO grantee-Data sets around Nike NFT collection-https://www.oceanmissions.com/data-packs/
-- Rome Blockchain Labs- Multi-chain DeFi data from GraphQL endpoint, activley want to list their data on Ocean Market
-- BloxRoute
-- Etherscan data, ideas by RealDataWhale https://www.reddit.com/r/CryptoCurrency/comments/yv642y/finding_opportunities_by_analyzing_etherscan_data/
+- [Ocean Missions](https://www.oceanmissions.com/data-packs/) Datasets around Nike NFT collection-
+- Rome Blockchain Labs - Multi-chain DeFi data from GraphQL endpoint, activley want to list their data on Ocean Market
+- BloxRoute -- mempool data
+- [RealDataWhale "Finding opportunities by analyzing Etherscan data"]( https://www.reddit.com/r/CryptoCurrency/comments/yv642y/finding_opportunities_by_analyzing_etherscan_data/)
 - (add to me)
 
+
+
+
```

### Comparing `predict_eth-0.1.1/ideas/modeling.md` & `predict_eth-0.1.2/ideas/modeling.md`

 * *Files identical despite different names*

### Comparing `predict_eth-0.1.1/predict_eth/helpers.py` & `predict_eth-0.1.2/predict_eth/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import time
 
 from brownie.network import accounts
 from brownie.network.account import LocalAccount
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
+
 from web3.main import Web3
 
 from ocean_lib.example_config import get_config_dict
 from ocean_lib.ocean.ocean import Ocean
 from ocean_lib.web3_internal.utils import connect_to_network
 
 # helper functions: setup
@@ -60,14 +61,20 @@
 
 def round_to_nearest_hour(dt: datetime.datetime) -> datetime.datetime:
     return dt.replace(
         second=0, microsecond=0, minute=0, hour=dt.hour
     ) + datetime.timedelta(hours=dt.minute // 30)
 
 
+def round_to_nearest_timeframe(dt: datetime.datetime) -> datetime.datetime:
+    return dt.replace(
+        second=0, microsecond=0, minute=(dt.minute // 5) * 5, hour=dt.hour
+    )
+
+
 def pretty_time(dt: datetime.datetime) -> str:
     return dt.strftime("%Y/%m/%d, %H:%M:%S")
 
 
 def print_datetime_info(descr: str, uts: list):
     dts = to_datetimes(uts)
     print(descr + ":")
@@ -79,14 +86,20 @@
 
 def target_12h_unixtimes(start_dt: datetime.datetime) -> list:
     target_dts = [start_dt + datetime.timedelta(hours=h) for h in range(12)]
     target_uts = to_unixtimes(target_dts)
     return target_uts
 
 
+def target_12_unixtimes(start_dt: datetime.datetime) -> list:
+    target_dts = [start_dt + datetime.timedelta(minutes=(m + 1) * 5) for m in range(12)]
+    target_uts = to_unixtimes(target_dts)
+    return target_uts
+
+
 # helper-functions: higher level
 def load_from_ohlc_data(file_name: str) -> tuple:
     """Returns (list_of_unixtimes, list_of_close_prices)"""
     with open(file_name, "r") as file:
         data_str = file.read().rstrip().replace('"', "")
     x = eval(data_str)  # list of lists
     uts = [xi[0] / 1000 for xi in x]
```

### Comparing `predict_eth-0.1.1/.gitignore` & `predict_eth-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `predict_eth-0.1.1/LICENSE` & `predict_eth-0.1.2/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Ocean Protocol
+Copyright (c) 2023 Ocean Protocol
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `predict_eth-0.1.1/pyproject.toml` & `predict_eth-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "hatchling",
   "hatch-requirements-txt",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "predict-eth"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Trent McConaghy", email="gtrent@gmail.com" },
 ]
 description = "Predict ETH challenges"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

