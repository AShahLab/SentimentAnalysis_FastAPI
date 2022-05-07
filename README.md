# SentimentAnalysis_FastAPI

## Step 1

Create a `FastAPI` Health Check endpoint:

1. Create a conda environment for holding onn the dependencies
2. Create a `main.py` file.
3. Add a `FastAPI` `get` route for `/health` which returns a string. This is the health check.

## Step 2

Create a `FastAPI` sentiment analysis endpoint:

1. Add imports for sentiment analysis model from huggingface.
2. Create a sentiment analysis pipeline.
3. Create a class for receiving the post request for sentiment analysis.
4. Add a route to handle post requests to `sentiment`,
5. In the above method pass the input string through the model.
6. Return the model results as the response.

## Step 3

Dockerize the code

1. Extract all dependencies from conda into `requirements.txt`.
2. Create a docker file from a slim python base.
3. Setup docker file to install all requirements, expose port 8000, and run uvicorn upon startup.
4. Create and tag docker file.
