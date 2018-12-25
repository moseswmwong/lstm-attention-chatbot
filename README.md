# lstm-attention-chatbot
Chatbot created in multi-level LSTM model with attention, training with movie conversations

This program provides an interesting chatbot which has many business and entertainment applications.

Model file can be downloaded [here](https://www.dropbox.com/s/6ybgdw6z0miq0nr/models.zip?dl=0)


## Preparations

1. Install Python, nVidia CUDA drivers, Google Tensorflow on a computer with GPU, e.g. nVidia GeForce GTX 1080, the system is created on a high performance Windows 10 platform using 1 nVidia GeForce GTX 1080, but it should works on Linux system with a high quality nVidia graphic card too. You should be able to run it on a CPU based system without GPU but the performance will not be very good. 
   - Tips: I used article from this link to build the Windows 10 PC and it is highly recommended installation guideline for the target AI system, please note that installing a Deep Learning PC is a complex process, so this installation guideline can save you much time. Click [The Best Way to Install TensorFlow with GPU Support on Windows 10](https://www.pugetsystems.com/labs/hpc/The-Best-Way-to-Install-TensorFlow-with-GPU-Support-on-Windows-10-Without-Installing-CUDA-1187/)
   - At this point you should be able to run a Python 3.x program under an Anaconda environment you had created, and run Tensorflow without problem. In particular, if you folllow the above installation guideline to build the AI system, you should be able to run the MINST training embedded inside Keras sucessfully and see the TensorBoard report on your browser.

2. Download all files from this repository

3. Create a subfolder 'datasets', and change directory to 'datasets' and create a subfolder 'cornell_movie_dialog'. Although these empyty folders are empty, they are required during chatbot startup.

4. Unzip the model file downloaded (as stated above). It should looks like this, first, a subfolder 'cornell_movie_dialog', and inside there is a trained model folder name in the format YYYYMMDD which indicate the date of model, and inside this folder there are multiple files:
   - best_weights_training.ckpt.* - Google tensorflow checkpoint files, you use best_weights_training.ckpt to launch the chatbot model in tensorflow.
   - cleaned_dataset - a text file that summaries all training data.
   - chat_logs - all your conversations with the chatbot can be found here.

## Running the chatbot

1. Open a command prompt

2. Change directory to this chatbot program

3. Activate <env_name>, where the env_name is the one you created in Preparation step 1. Note that activate is an Anaconda program for you to enable a specific Data Science environment, e.g. Python 3.6 with CUDA 9.0 and Tensorflow 1.10.0

4. Run this command
   - python chat.py models\cornell_movie_dialog\20181223\best_weights_training.ckpt



