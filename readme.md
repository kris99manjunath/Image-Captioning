#INTRODUCTION:
A image captioning model made using inceptionV3,glove and flickr8k dataset

## PROPOSED SYSTEM:
Image captioning is a new technology that combines LSTM text generation with the computer vision powers of a convolutional neural network.
Here we will make use of LSTM and CNN to create a basic image captioning system. 
Inception is used to extract features from the images. Glove is a set of Natural Language Processing (NLP) vectors for common words.

There are two neural networks that are accessed via transfer learning.
 
It is important to understand that a caption is not generated with one single call to the neural network's predict function. Neural networks output a fixed-length tensor. To get a variable length output, such as free-form text, requires multiple calls to the neural network.
The neural network accepts two objects (which are mapped to the input neurons). The first is the photo. The second is an ever growing caption. The caption begins with just the starting token. The neural network's output is the prediction of the next word in the caption. This continues until an end token is predicted or we reach the maximum length of a caption. Each time predict a new word is predicted for the caption. The word that has the highest probability (from the neural network) is chosen

 
