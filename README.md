# USAmin 2

Project Type: Independent 

# Motivation

After learning about how the usefulness of deep learning packages Python and Keras provides, I was eager to optimize the first NLP and deep learning project I ever worked on. But, only optimizing the project was not enough for me. I wanted to apply the techniques I have learned about deep learning into this project to see if there is any improvement in the model's predictions.

# Summary

This is an independent project which takes the ideas of [USAmin](https://github.com/yuj072/USAmin) and incorporates the methods I learned from competing in the [Jigsaw toxicity classification contest](https://github.com/yuj072/toxicity-classification).

# Changes

- Used deep learning packages to aid in obtaining word embeddings, defining training and test sets, and performing validation.
- Added a Spatial Dropout Layer inside of the LSTM.
- The LSTM is bidirectional and returns the tensor at every timestep (return_sequence=True)
- Added a Global Average Pooling Layer between the LSTM and MLP
- Added a Global Max Pooling Layer between the LSTM and MLP
- MLP now takes in a concatenated tensor of Spatial Dropout, Global Average Pooling, Global Max Pooling, and the collection of tensors returned by the LSTM in order to predict the review score.
- Added KFold Validation

# Results

Using the same metrics for accuracy as [USAmin](https://github.com/yuj072/USAmin):

<img src="https://latex.codecogs.com/gif.latex?Math.abs(predicted&space;-&space;actual)&space;<=&space;0.25">

the same results (~20% accuracy) were obtained. This reinforces the conclusion we reached at the end of the [USAmin](https://github.com/yuj072/USAmin) project: _There appears to be a very weak correlation between a movie's summary and average rating._

