# SageMaker Deployment Project

This project is building and deployment of a sentiment analysis of movie reviews. The reviews are classified as simply positive or negative.

The project is not very complicated, but the point of the project is to embedd the model in a Flask webapp and to deploy it on the AWS SageMaker server.

### Project Breakdown

This project is divided into 3 parts.

1. [Train ](https://github.com/mohammadjafri1992/SentimentAnalysisWebApp/tree/master/train)
2. [Serve](https://github.com/mohammadjafri1992/SentimentAnalysisWebApp/tree/master/serve)
3. [Website](https://github.com/mohammadjafri1992/SentimentAnalysisWebApp/tree/master/website)

Our website is a simple HTML page running on a python micro web framework. You can see the website [here](https://github.com/mohammadjafri1992/SentimentAnalysisWebApp/blob/master/website/index.html).

For the training part of the problem, I trained the given data using two files; [model.py](https://github.com/mohammadjafri1992/SentimentAnalysisWebApp/blob/master/train/model.py) and [train.py](https://github.com/mohammadjafri1992/SentimentAnalysisWebApp/blob/master/train/train.py).

