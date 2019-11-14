# SentimentAnalysisWebApp

This is web app which classifies a movie review to be either positive or negative. The algorithm used is based on [Bag of Words model](https://en.wikipedia.org/wiki/Bag-of-words_model).

The web app is very simple. It is essentially an HTML document with ability to POST raw data (review in our case) to the API as shown in the HTML code file (index.html).

Detailed description of the model and its implementation can be viewed in the following blogpost on Medium.

### Model Description

The model is a basic RNN implementation. It is deployed on AWS SageMaker services with the model endpoints accessable by the users through an API Gateway created with IAM configurations to allow everyone to use the model.

Deploying the API creates a secured web address which is used as the POST request "action" in the HTML webpage.

All model details are available on the blog post.

Hope you enjoy reading the model.

## DISCLAIMER
This project is issued under MIT License. Under no circumstances is the author liable for any loss/damage/alteration (permanent or temporary), to the computer system including software and hardware. AWS is a service managed by Amazon. Please see their guidelines for hosting and/or deploying your model. AWS is a paid service.
