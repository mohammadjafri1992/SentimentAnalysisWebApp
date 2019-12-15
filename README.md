# SageMaker Deployment Project

This project is building and deployment of a sentiment analysis of movie reviews. The reviews are classified as simply positive or negative.

The project is not very complicated, but the point of the project is to embedd the model in a Flask webapp and to deploy it on the AWS SageMaker server.

## Project Breakdown

This project is divided into 3 parts.

1. [Train ](https://github.com/mohammadjafri1992/SentimentAnalysisWebApp/tree/master/train)
2. [Serve](https://github.com/mohammadjafri1992/SentimentAnalysisWebApp/tree/master/serve)
3. [Website](https://github.com/mohammadjafri1992/SentimentAnalysisWebApp/tree/master/website)

### Website
Our website is a simple HTML page running on a python micro web framework. You can see the website [here](https://github.com/mohammadjafri1992/SentimentAnalysisWebApp/blob/master/website/index.html). In the last <div> of the html file, where  the form method is POST, I replaced the "action" text "*REPLACE WITH PUBLIC API URL*" with my API endpoint. Since i dont have the project active anymore, I removed the Public API link and reverted the text back to "*REPLACE WITH PUBLIC API URL*"

### Training
For the training part of the problem, I trained the given data using two files; [model.py](https://github.com/mohammadjafri1992/SentimentAnalysisWebApp/blob/master/train/model.py) and [train.py](https://github.com/mohammadjafri1992/SentimentAnalysisWebApp/blob/master/train/train.py). 

Model.py contains the code for LSTMClassifier model built using PyTorch.

Train.py contains the training code developed in the [Jupyter notebook](https://github.com/mohammadjafri1992/SentimentAnalysisWebApp/blob/master/SageMaker%20Project.ipynb).

### Serving
After the data was trained using train.py code, the model needs to serve the predicted values. This is performed by the [predict.py](https://github.com/mohammadjafri1992/SentimentAnalysisWebApp/blob/master/serve/predict.py) file.

I would highly recommend to look at the files to see the comments and other code annotations, line-by-line. That would make much more sense rather than just reading about it here.

### Disclaimer
It is website is available as an open source with MIT license. To reiterate, the code is provided AS-IS. I am not responsible for any loss/damage caused by the code to your hardware, software or business in any shape or form. This code is provided for educational purpose ONLY and must not be taken as a business proposal. Running this code on AWS will incurr charges.

