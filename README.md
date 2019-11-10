# Project 3 Generative Audio

Chandhini Grandhi, cgrandhi@ucsd.edu


## Abstract

In this project, I am planning to produce audio based on emotions detected from tweets. The architecture consists of three phases:<\br >
1. Perform Sentiment analysis on data and classify the emotion of the tweet. I used Random Forest Classifier to achieve this and I am only considering the two emotions- happiness, sadness<\ br>
2. Perform Text-to-Speech synthesis by using a tacotron model for the tweet entered. <\br >
3. Generate new audio based on the emotion detected by using a Wavenet Model.<\br >

I am using a pretrained Tacotron model discussed in class. I trained the Wavenet model on the following emotional-audio dataset https://www.kaggle.com/uwrfkaggler/ravdess-emotional-speech-audio. This project can be extended to audio style transfer where it can detect the emotion and perform style transfer on the audio to concatenate the original audio with a stylized audio. 

## Model/Data

Briefly describe the files that are included with your repository:
- trained models
- training data (or link to training data)

## Code

Your code for generating your project:
- Python: generative_code.py
- Jupyter notebooks: generative_code.ipynb

## Results

Documentation of your results in an appropriate format, both links to files and a brief description of their contents:
- `.wav` files or `.mp4`
- `.midi` files
- musical scores
- ... some other form

## Technical Notes

Any implementation details or notes we need to repeat your work. 
- Does this code require other pip packages, software, etc?
- Does it run on some other (non-datahub) platform? (CoLab, etc.)

## Reference

References to any papers, techniques, repositories you used:
- Papers
- Repositories
- Blog posts
