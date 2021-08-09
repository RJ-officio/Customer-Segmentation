# Personality Traits Analysis among Social Media Influencers with LSTM

The idea of this project is to build a sentiment analysis model that detects the emotions that underlie a tweet. It makes associations between words and emotions and the aim is to classify the tweets into sentiments like anger, happiness, sadness, enthusiasm etc. rather than the usual sentiment classification that only involves truly contrasting sentiments of Positive and Negative.

## The Data:
The data can be downloaded from tweetdata.csv file.

## Files:
The repository contains 3 python scripts. 
lstm_personalitytraits.py contains the data pre-processing code. 
model_traits.py contains the trained LSTM model.
main.py contains a Flask api that posts desired sentence and fetches the predicted sentiment model from the LSTM model.
model.h5 contains the saved keras model of LSTM.

## Overview:
This github repository can be cloned with the following command in your cmd : "https://github.com/jaiobs/Personality-Traits-Analysis" \n
Move to the respective directory.
pip install the requirements.txt with the following command in your python environment. "pip install -r requirements.txt"
Once the requirements are loaded, run the main.py program with the command - "python main.py"
Once the script is done running, the API starts running in the respective port mentioned in the "main.py" file.
Copy the API address and run it in Postman Application. (eg. http://127.0.0.1:5009/personality)
Change the method to POST and choose the from-data option from Body. Give the desired text in the Value column and "text" as Key.
Send the request to fetch the predicted sentiment as a response from the LSTM model in raw format.

