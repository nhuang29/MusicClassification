# MusicClassification
This is a repo containing research and coding of Music Classification using Tensorflow's Keras. The two main classifications in progress here are genre classification and mood classification. Mood Classification coming soon! 

Technologies Used:
- Jupyter Notebook
- Python

Terminology Used:
- CNN (Convolutional Neural Network)
- RNN (Recurrent Neural Network
- NN (Neural Network)
- FFT (Fast Fourier Transform)
- STFT (Short Time Fourier Transform)

Packages Used:
- numpy
- librosa
- json
- scikit learn
- tensorflow
- matplotlib
- ffmpeg

## Explaination of Each Package and it's uses:
1.) <ins>Numpy</ins>: Numpy is one of the most famous libraries in Python. I used numpy to help load data into a digestible state for Scikitlearn.

2.) <ins>Ffmpeg</ins>: This library library allows for the loading of data of various formats (MP3, OGG, Flac) to librosa

3.) <ins>Librosa</ins>: Librosa is an audio file feature extraction library built in Python. Librosa was used to extract important features about the audio file. For example, an MFCC Coefficient, which shows frequency amplitude based on human hearng was extracted for analysis. To learn more about Librosa here's a great [article](https://medium.com/coderhack-com/introduction-to-librosa-912c2c109f41#:~:text=LibROSA%20is%20a%20Python%20package%20for%20audio%20and%20music%20analysis,%2C%20MP3%2C%20FLAC%2C%20etc.)! 

4.) <ins>Json</ins>: This library is used to read/write/manipulate json files. The json package was used to provide structured data to the machine learning model of keras for analysis.

5.) <ins>Scikit learn</ins>: This library is a famous machine learning library. In the code, I used this to split my dataset into a training/testing/validation set. I'll explain in a little bit why this is important.

6.) <ins>Tensorflow</ins>: Tensorflow is one of the most famous machine learning libraries. Here, I used it to be able to quickly spin up a model (using keras) and train the model with the data that was extracted from each audio file 

7.) <ins>Matplotlib</ins>: Matplotlib is another well known library for being able to plot out and provide visual representations of data. I used this library to be able to show a step by step of what data should look like. This helped me in 
visualizing what I was turning the audio files into (Frequency vs Time, Amplitude vs Time, etc.)

## Recommended Steps for Going Through The Repo:
**Step 1**: Please proceed to the "Learning" subdirectory. This is a walkthrough of all the pieces that we will be building. It will lead to better understanding of how Librosa works and how neural networks work

**Step 2**: Proceed to the Genre Classification section. There you will see a preprocess file, a CNN classification file, and a NN classification file (named MusicGenreClassifier). This is where you can test on your own set of data. The "Instructions" file will explain how to run this and what differentiates the CNN from a regular NN

## Notes:

**IMPORTANT**: I wrote this in Jupyter Notebook. It can be run in PyCharm and any environment you please. 

**IMPORTANT**: The data that I used for this can be obtained through this URL: [Gatzen Music Classification Data Set](https://www.kaggle.com/datasets/carlthome/gtzan-genre-collection). It has a famous dataset that includes 10 different genres. Note that each clip isn't exactly a "whole song". That way, if you are running your model via your computer's CPU, the results will appear rather quickly. The files are also on this github in the Music Genre Classification subdirectory.
