# Predicting a customer's next purchase using automated feature engineering



**As customers use your product, they leave behind a trail of behaviors that indicate how they will act in the future. Through automated feature engineering we can identify the predictive patterns in granular customer behavioral data that can be used to improve the customer's experience and generate additional revenue for your business.**

In this tutorial, we show how  can be used to perform feature engineering on a multi-table dataset of 3 million online grocery orders provided by Instacart to train an accurate machine learning model to predict what product a customer buys next.

*Note: If you are running this notebook yourself, refer to the read me on Github for instructions to download the Instacart dataset*

## Highlights

* We automatically generate 150+ features using Deep Feature Synthesis and select the 20 most important features for predictive modeling
* We build a pipeline that it can be reused for numerous prediction problems (you can try this yourself!)
* We quickly develop a model on a subset of the data and validate on the entire dataset in a scalable manner using [Dask](http://dask.pydata.org/en/latest/).

## Running the tutorial


1. Install the requirements

    ```
    pip install -r requirements.txt
    ```
    
    *You will also need to install **graphviz** for this demo. Please install graphviz .
    
2. Download the data

    You can download the data directly from Instacart [here](https://www.instacart.com/datasets/grocery-shopping-2017).

    After downloading the data save the CSVs to a directory called `data` in the root of this repository. Then run the following command in your terminal from the root of this repo.

    ```
    >> python process_data.py
     70%|██████████████████████████▌           | 145/207 [07:43<03:18,  3.20s/it]
    ```
    *Note: Expect this command to take up to 20 minutes to run as it prepares the data for the tutorial notebook*

3. Run the [Tutorial](Tutorial.ipynb) using Jupyter

    ```
    jupyter notebook
    ```

### Contact

Any questions can be directed to 1729231@kiit.ac.in
