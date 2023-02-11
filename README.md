![pexels-pixabay-158651](https://user-images.githubusercontent.com/100870737/218273182-11ce169b-aa79-4176-9b2b-e81dad7164c3.jpg)


## MLOps News Data Classification NLP Model
MLOps Project for NLP Model with Data from AG News is a collection of more than 1 million news articles gathered from more than 2000 news sources by an academic news search engine


- ## Part 1:
  - Project: machine learning text classifier to predict news categories from the news article text.
    - Iterated on classification models with increasing level of complexity and improved performance
    - Analyzed the impact of training data size on model performance

- ## Part 2:
  - Project: detailed model evaluation, data quality testing, and behavioral testing for the news classification model from part 1
    - Analyzed evaluation metrics beyond overall accuracy and f1 score (per-class metrics, confusion matrix, per-class false positive and false negative errors)
    - Implemented bootstrap sampling to measure confidence intervals of model performance metrics
    -  Implemented behavioral tests using a popular open source library called checklist

- ## Part 3:
  - Project: Model deployment for the news classification model that we trained in part 1, and evaluated in part 2
    - Built a simple web application backend using FastAPI and Uvicorn that wraps the trained model, and exposes an endpoint to make predictions on live traffic that is sent to the endpoint
    - Wrapped the application in a Linux container using Docker. This will make it easier to deploy to a cloud environment later.
    - Tested the Dockerized prediction service by sending it live traffic and logging the model predictions

- ## Part 4:
  - Project: Focused on model performance monitoring for the news classification model that was deployed in part 3
    - Downloaded and parsed the training dataset, logs from prediction service that record inference traffic and annotations (ground truth labels for the inference traffic)
    - Set up basic monitoring for system health (traffic volume, latency, SLA violations)
    - Computed data and label drift for the inference traffic using a few different techniques (Chi-square statistic, KS-statistic, classifier-based drift detection)
    - Analyzed model performance as a function of time for the inference traffic, and any ties we can derive to detected drift
