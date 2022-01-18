# Emotion Classification on SemEval 2019 Task 3

## Project Description

Emotion is often defined as individual's mental, and has been increasingly researched in many fields. In general, recognizing emotion could bring profits to customer services, psychology, sociology, etc. However, Emotion Recognition is not an easy task, even well trained human service people are struggle to do so. In this project, we implement RNN based Deep Neural Network, fine-tuned the models, and investigate their performance.

## Project Structure

1. baseline model: use CLS vector of Bert as sentence embedding, and feed to a dense layer
2. glove_lstm model: use each word's embedding as input, bidirectional lstm as encoder, and dense network as decoder. Feed the encoder with three utterances separately first and then concatenate them together for decoder
3. bert_lstm model: neural network structure is the same as glove_lstm, and we use bert as word embeddings
