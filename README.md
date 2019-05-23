# USAmin 2

Project Type: Independent 

# Quick Summary
This is an independent project which takes the ideas of [USAmin](https://github.com/yuj072/USAmin) and incorporates the methods I learned from competing in the [Jigsaw toxicity classification contest](https://github.com/yuj072/toxicity-classification).

# Changes
- Used deep learning packages to aid in obtaining word embeddings, defining training and test sets, and performing validation.
- Added a Spatial Dropout Layer inside of the LSTM.
- Added a Global Average Pooling Layer between the LSTM and MLP
- Added a Global Max Pooling Layer between the LSTM and MLP
- Added KFold Validation

# Results
Using the same metrics for accuracy as [USAmin](https://github.com/yuj072/USAmin):

<img src="https://latex.codecogs.com/gif.latex?Math.abs(predicted&space;-&space;actual)&space;<=&space;0.25">

the same results (~20% accuracy) were obtained. This reinforces the conclusion we reached at the end of the [USAmin](https://github.com/yuj072/USAmin) project: _There is a very weak correlation between a movie's summary and average rating._

