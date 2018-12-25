# lstm-attention-chatbot
Chatbot created in multi-level LSTM model with attention, training with movie conversations

This program provides an interesting chatbot which has many business and entertainment applications.

Model file can be downloaded [here](https://www.dropbox.com/s/6ybgdw6z0miq0nr/models.zip?dl=0)


## Preparations

1. Create a subfolder 'datasets', and change directory to 'datasets' and create a subfolder 'cornell_movie_dialog'. Although these empyty folders are empty, they are required during chatbot startup.

2. Unzip the model file downloaded (as stated above). It should looks like this, first, a subfolder 'cornell_movie_dialog', and inside there is a trained model folder name in the format YYYYMMDD which indicate the date of model, and inside this folder there are multiple files:

    2.1 best_weights_training.ckpt.*
        Google tensorflow checkpoint files, you use best_weights_training.ckpt to launch the chatbot model in tensorflow.
        
    2.2 cleaned_dataset
        A text file that summaries all training data.
        
    2.3 chat_logs
        All your conversations with the chatbot can be found here.
