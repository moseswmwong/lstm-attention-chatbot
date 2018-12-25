# lstm-attention-chatbot
Chatbot created in multi-level LSTM model with attention, training with movie conversations

This program provides a basic chatbot

model file can be downloaded [here](https://www.dropbox.com/s/6ybgdw6z0miq0nr/models.zip?dl=0)


## Preparations

1. create a subfolder 'datasets', and change direction to 'datasets' and create a subfolder 'cornell_movie_dialog'. Although these empyty folders are not used, they are required during chatbot startup.

2. unzip the model file. It should looks like this, first, the subfolder 'cornell_movie_dialog', and inside there is a trained model name in the format YYYYMMDD which indicate the date of model training started, and inside this folder there are multiple files:

    2.1 best_weights_training.ckpt.*
    
    2.2 cleaned_dataset
