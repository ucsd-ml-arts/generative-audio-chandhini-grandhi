# Project 3 Generative Audio

Chandhini Grandhi, cgrandhi@ucsd.edu


## Abstract

In this project, I am planning to produce audio based on emotions detected from tweets. The architecture consists of three phases:
1. Perform Sentiment analysis on data and classify the emotion of the tweet. I used Random Forest Classifier to achieve this and I am only considering the two emotions- happiness, sadness
2. Perform Text-to-Speech synthesis by using a tacotron model for the tweet entered. 
3. Generate new audio based on the emotion detected by using a Wavenet Model.

I am using a pretrained Tacotron model discussed in class. I trained the Wavenet model on the following emotional-audio dataset https://www.kaggle.com/uwrfkaggler/ravdess-emotional-speech-audio. This project can be extended to audio style transfer where it can detect the emotion and perform style transfer on the audio to concatenate the original audio with a stylized audio. 

## Model/Data

Dataset: The Data folder contains the following:
1. text_emotion.csv - Labelled dataset of tweets and emotions
2. Sad_audio - A collection of sad audio spoken by 24 speakers obtained from [RAVDESS](https://www.kaggle.com/uwrfkaggler/ravdess-emotional-speech-audio)
3. Happy audio -  A collection of happy audio spoken by 24 speakers obtained from [RAVDESS](https://www.kaggle.com/uwrfkaggler/ravdess-emotional-speech-audio)

Models:
Tacotron2 - As discussed in class, I used the inference model from NVIDIA's repository https://github.com/NVIDIA/tacotron2
Wavenet - The official implementation of the paper 'Wavenet generative neural network architecture' is available here https://github.com/ibab/tensorflow-wavenet . I followed the commands to trained the model on my dataset.

## Code
The project can be generated by running the following code:
1. Text-Classification/Emotion-classification.ipynb : This code performs sentiment analysis and classifies emotion. Then stores the emotion detected along with the tweet given as input in shared files.
2. tacotron/inference.ipynb : Loads the pretrained models of tacotron and wavenet and get the tweet entered from the shared file and converts it into speech
3. tensorflow/wavenet : Trains the wavenet on the audio files available and generates new audio.

## Results
Sample output: 

Tweet = 'This is quite depressing. I am filled with sorrow'<br />
Emotion classification output : sadness<br />
Tacotron output: 
Wavenet output: 
![Alt Text]()


## Technical Notes

The project runs on Google colab


## Reference

References to any papers, techniques, repositories you used:
- Papers
- Repositories
    - https://github.com/NVIDIA/tacotron2
    - https://github.com/ibab/tensorflow-wavenet
- Blog posts
    - https://deepmind.com/blog/article/wavenet-generative-model-raw-audio
