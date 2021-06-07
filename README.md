# Music Style Transfer

Members: Haojun Li (haojun), Gavin Zhang (jzhang07)

Team Contributions:

Haojun - Preprocessing. Dilated CNN modeling and experiments and LSTM experiments. Feature extraction. Poster lead.

Gavin Zhang - Report lead and composition. Generating LSTM results.

## Introduction
The problem we are investigating is whether it is possible to transfer music style from one genre of music to another. We have come to realize that that there are many ways of transferring style, from dynamics (how the volume changes over time) to rhythm (tempo of the music) to pitch (music scores differences). Our work drew inspiration from this [paper](https://arxiv.org/pdf/1708.03535.pdf), which attempts to learn the dynamics of classical and jazz piano pieces. We expand upon their investigations of learning the dynamics of a piece by using dilated CNN (wavenet) and including chords generations.

## Project Format
The project is structed in 3 notebooks. The Preprocessing notebook contains code that splits a midi music into 3 distinct matrices. The Dilated CNN notebook contains code to generate velocity information. The LSTM notebook contains code that trains a different CNN, and then use the features encoded as activations of the CNN to generate music through LSTM. Since LSTM takes a long time to run, both Haojun and Gavin have run the training code by sharing weights.

## References
1. [Tonenet](https://medium.com/@suraj.jayakumar/tonenet-a-musical-style-transfer-c0a18903c910)
2. [Stylenet](https://github.com/imalikshake/StyleNet/)
3. [Wavenet](https://deepmind.com/blog/wavenet-generative-model-raw-audio/)
