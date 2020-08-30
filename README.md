# Creating a Sentiment Analysis Web App
## Using PyTorch and SageMaker

_[Machine Learning Engineer Nanodegree Program](https://www.udacity.com/course/machine-learning-engineer-nanodegree--nd009t) | Deployment_

## General Outline
**general outline for SageMaker projects using a notebook instance.**

1. Download or otherwise retrieve the data.
2. Process / Prepare the data.
3. Upload the processed data to S3.
4. Train a chosen model.
5. Test the trained model (typically using a batch transform job).
6. Deploy the trained model.
7. Use the deployed model.

For this project, I followed the steps in the general outline with some modifications.

First, I didn't test the model in its own step. we deployed the model and then tested it by sending the test data to it. One of the reasons for doing this is so that I can make sure that the deployed model is working correctly before moving forward.

In addition, I deployed and used the trained model a second time. In the second iteration I customized the way that my trained model is deployed by including some of my own code. In addition, my newly deployed model is used in the sentiment analysis web app.

## Files

- [SageMaker Project](https://github.com/ahmed-gharib89/deploy-sentiment-analysis-model/blob/master/SageMaker%20Project.ipynb): is the main notebook that we run in AWS SageMaker and use SageMaker features to creat, train and deploy our model
- serve folder contains the files needed for our model to be deployed
  - [model.py](https://github.com/ahmed-gharib89/deploy-sentiment-analysis-model/blob/master/serve/model.py)
  - [predict.py](https://github.com/ahmed-gharib89/deploy-sentiment-analysis-model/blob/master/serve/predict.py)
  - [utils.py](https://github.com/ahmed-gharib89/deploy-sentiment-analysis-model/blob/master/serve/utils.py)
  - [requirements.txt](https://github.com/ahmed-gharib89/deploy-sentiment-analysis-model/blob/master/serve/requirements.txt)
- train folder contains the files needed to deploy and test our first model
  - [model.py](https://github.com/ahmed-gharib89/deploy-sentiment-analysis-model/blob/master/train/model.py)
  - [train.py](https://github.com/ahmed-gharib89/deploy-sentiment-analysis-model/blob/master/train/predict.py)
  - [requirements.txt](https://github.com/ahmed-gharib89/deploy-sentiment-analysis-model/blob/master/train/requirements.txt)
- website folder contains only the html file of our simple web app
  - [index.html](https://github.com/ahmed-gharib89/deploy-sentiment-analysis-model/blob/master/website/index.html)


#### Find me in social media
[![Github](https://img.icons8.com/ios-filled/30/000000/github.png "Github")](https://github.com/ahmed-gharib89 "Github")
[![LinkedIn](https://img.icons8.com/ios-glyphs/30/000000/linkedin.png "LinkedIn")](https://www.linkedin.com/in/ahmed-abdel-moniem-gharib/ "LinkedIn")
[![Facebook](https://img.icons8.com/ios-filled/30/000000/facebook-new.png "Facebook")](https://www.facebook.com/just.nimo/)
[![Whatsapp](https://img.icons8.com/ios/30/000000/whatsapp.png "Whatsapp")](https://wa.me/201096995535?text=Hello)
[![Instagram](https://img.icons8.com/ios/30/000000/instagram.png "Instagram")](https://www.instagram.com/ahmed.gharib89/)

 
