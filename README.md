# :chart_with_upwards_trend: Masterclass - Introduction to Time Series Forecasting

![](https://github.com/MKB-Datalab/workshop_ts_forecasting/blob/master/images/aron-visuals-BXOXnQ26B7o-unsplash.jpg)
Photo by <a href="https://unsplash.com/@aronvisuals?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Aron Visuals</a> on <a href="https://unsplash.com/@aronvisuals?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>

This repository contains support material used during the Masterclass Introduction to Time Series Forecasting offered by [JADS MKB datalab](https://www.jadsmkbdatalab.nl/) to [JADS'](https://www.jads.nl/) students.

During these hands-on session students learn some some basics about time series and SARIMAX and Facebook Prophet models. We will explore topics such as:

* What is Forecasting?
* Some applications of Forecasting
* What is Time Series ?
* Time Series components
* Introduction to ARIMA models (non-seasonal and seasonal ARIMA)
* Introduction to Facebook forecasting model PROPHET

After completing this workshop, you will be able to identify time series and its properties using both statistical and graphical tools. You will be able to start applying ARIMA models and their variants SARIMA and ARIMAX: statistical models used for forecasting. Last but not least, you will get to know Facebook Prophet so you can start applying it and go further exploring it with different use cases.
  
Furthermore, during this session we present some real datasets and some challenges that might be encountered when working with real data.

## :file_folder: Data

In the pratical examples we used the following data:

1. Data obtained from [Google Trends](https://trends.google.com/trends/). This data can be found [here](https://github.com/MKB-Datalab/workshop_ts_forecasting/tree/master/data/google_trends).

2. The data referent to search of the word `diet` in USA was expanded and can be found [here](https://github.com/MKB-Datalab/workshop_ts_forecasting/blob/master/data/processed/diet_USA_2016_2023.csv).

3. [global temperature dataset time series](https://datahub.io/core/global-temp#data). This dataset includes global monthly mean temperature anomalies in degrees Celsius from 1880 to the present. Data are included from the GISS Surface Temperature (GISTEMP) analysis and the global component of Climate at a Glance (GCAG). This data can be found [here](https://github.com/MKB-Datalab/workshop_ts_forecasting/blob/master/data/monthly_csv.csv).

4. Data from Kaggle's competition [**Store Item Demand Forecasting Challenge**](https://www.kaggle.com/c/demand-forecasting-kernels-only) which consists of 5 years of store-item sales data split in a training dataset (train.csv) and a test dataset (test.csv). 

More specifically, in our examples, we used a part of this data that can be found [here](https://github.com/MKB-Datalab/workshop_ts_forecasting/tree/master/data/processed).

## Material workshop

* Workshop presentation: [time_series_v230423.pptx](https://github.com/MKB-Datalab/workshop_ts_forecasting/blob/master/docs/time_series_v230423.pptx)
* Exercises covered during workshop and answers of those can be found at [notebooks/Exercises](https://github.com/MKB-Datalab/workshop_ts_forecasting/tree/master/notebooks/Exercises)

The following notebooks present more details about what we covered together.

In **[01-Intro_time_series_tutorial_v220423.ipynb](https://github.com/MKB-Datalab/workshop_ts_forecasting/blob/master/notebooks/01-Intro_time_series_tutorial_v220423.ipynb)** you learn about time series properties and how to identify them using both statistical and graphical tools.

Next, in **[02-Forecasting_with_SARIMAX.ipynb_v220423](https://github.com/MKB-Datalab/workshop_ts_forecasting/blob/master/notebooks/02-Forecasting_with_SARIMAX.ipynb_v220423)** you are introduced to ARIMA models and its variants. There we apply SARIMA model on a [store-item sales data](https://www.kaggle.com/c/demand-forecasting-kernels-only) and forecast the sales 3 months in the future.

In the last notebook, **[03-Forecasting_with_Facebook_Prophet_v220423.ipynb](https://github.com/MKB-Datalab/workshop_ts_forecasting/blob/master/notebooks/03-Forecasting_with_Facebook_Prophet_v220423.ipynb)**, we introduce Facebook Prophet. We compare it with other models such as SARIMAX and apply it to the same dataset. We finalize by comparing the performance of all models obtained (SARIMA and Prophet models).

 
## Pre-requesits

:white_check_mark: Knowledge of Python

:white_check_mark: Dowload data in [data/google_trends](https://github.com/MKB-Datalab/workshop_ts_forecasting/tree/master/data/google_trends) and in [data/processed](https://github.com/MKB-Datalab/workshop_ts_forecasting/tree/master/data/processed)

:white_check_mark: The following are the most important libraries we will be using and the versions that were used. Be sure you have them running:

:wrench: numpy == 1.21.4

:wrench: pandas == 1.2.4

:wrench: matplotlib == 3.3.4

:wrench: seaborn == 0.11.1

:wrench: statsmodels==0.12.2

:wrench: prophet==1.1.2

:wrench: joblib==1.0.1

:wrench: pmdarima==1.8.2

## :computer: Install requirements
* The libraries above with versions are in so you can also install using: Install requirements using `pip install -r time_series_requirements.txt`.
  * Make sure you use Python 3 (I'm using 3.8.5).
  * My version of Conda 4.10.1
  * You may want to use a virtual environment for this.

-------------------------------------
[:arrow_backward: **Back to repository main page**](https://github.com/MKB-Datalab/mkbdatalab_knowledge_repository_main)