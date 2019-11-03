# Project 3 Generative Audio

Chandhini Grandhi, cgrandhi@ucsd.edu


## Abstract

Include your abstract here. This should be one paragraph clearly describing your concept, method, and results. This should tell us what architecture/approach you used. Also describe your creative goals, and whether you were successful in achieving them. Also could describe future directions.

In this project, I am planning to produce audio/speech based on user's emotions. The architecture consists of two phases- first to classify and detect the emotion of the user and the second model will generate audio based on the emotion detected. I am still figuring out on where to obtain the text data to train the model but once I have it, I will use a normal classifier to parse the data and detect the emotion. The emotion detected will then be fed to a Wavenet based model which can generate new audio. The dataset I am going to use to train the audio/speech samples is available here https://www.kaggle.com/ejlok1/toronto-emotional-speech-set-tess. I am planning to get the user to enter a 50-word text about his feeling for the day and detect the emotion from the text enterted as it would be more real-time this way. 

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
