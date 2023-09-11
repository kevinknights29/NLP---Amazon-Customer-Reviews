# NLP: Amazon Customer Reviews

This project which seeks to predict the rating of a text review using NLP algorithms and the Amazon Customer Reviews dataset.

## Objectives

- Create a model capable of predicting customer satisfaction from information available in the form of comments and articles.

## Dataset description

The dataset contains the customer review text with accompanying metadata, which consists of three main components:

- A collection of reviews written on the Amazon.com marketplace and associated metadata from 1995 to 2015. This is intended to facilitate the study of the properties (and evolution) of customer reviews, potentially including how people evaluate and express your experiences with scale products. (130M + customer reviews)

- A collection of multi-lingual product reviews from different Amazon marketplaces, intended to facilitate analysis of customer perceptions of the same products and broader consumer preferences in all languages ​​and countries. (More than 200K customer reviews in 5 countries)

- A collection of reviews that have been identified as non-compliant with respect to Amazon policies. This is intended to provide a baseline data set for research on detecting promotional or biased reviews. (several thousand customer comments). This part of the data set is distributed separately and is available on request; Please contact the email address below if you are interested in obtaining this dataset.

## Usage

To run this project's code you can leverage Docker with the instructions below:

1. For first time usage, you need to build the Docker image:

    ```bash
    docker compose build .
    ```

2. After that you can start the container with:

    ```bash
    docker compose up -d
    ```

3. Go to Docker desktop, to retrieve your jupyterlab access URL.

    - Click the container name, to open the logs.
    - Retrive the jupyterlab URL, it should look like: `http://127.0.0.1:8888/lab?token=4150032f3603c85febf54b8b40bb761a2eb46e2fb593d5dc`

    ![image](https://github.com/kevinknights29/Airflow_Docs_LLM_App/assets/74464814/661f3747-2b2e-4387-9c79-64af1d8bc56e)

4. To stop the container, run:

    ```bash
    docker compose down
    ```

## Project Conclusions

- The model can still be optimized by improving its hyperparameters.
- By balancing the dataset we can expect better results.
- The training dataset was delimited for reasons of computational resources, we can estimate that with a greater number of records and columns of the DTM the model will have a greater predictive power.
- I consider that the model obtained a good performance, taking into account the previous limitations.
