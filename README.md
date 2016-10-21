# Problem Statement: 
Compute Steering Angle for keeping a self-driving car in a lane, given a single camera image as input. Read more at [Udacity Challenge 2 Blog](https://medium.com/udacity/challenge-2-using-deep-learning-to-predict-steering-angles-f42004a36ff3#.bx1vjl4he)

# Solution 
## Nvidia-End-to-End Learning Deep Neural
A TensorFlow implementation of this [Nvidia paper](https://arxiv.org/pdf/1604.07316.pdf) with some changes.

## How to Use
Use `python train.py` to train the model

Use `python run.py` to run the model on a live webcam feed

Use `python run_dataset.py` to run the model on the dataset

## Download Dataset 
  Download a [Udacity Dataset](https://github.com/udacity/self-driving-car) and extract into a (new) $REPO_ROOT/dataset folder

## Extration
  Use [Udacity ROS Reader](https://github.com/rwightman/udacity-driving-reader) repository to extract the dataset using Docker containers. 
  
## Status

As of October 15:
- [x] Started: October 10, 2016
- [x] Got the environment up and running (on MacOS host)
- [x] Successfully trained a NN using a open source implementation of nVidia-end-to-end-learning network (took ~9 hours)
- [x] Upgraded to nVidia-Cuda Multi Core Hardware which brought training time down to ~1 hour
- [x] Trained model using Udacity Sunny data from 09/29/2016 (12:40 mins)
  - [x] RMSE was too low
  - [x] Model was overfit
- [ ] WIP: Filter training to kill low speed and steep steering angles
- [ ] Prepare Training Data with Scene Augmentation for drift recovery training
- [ ] Move Dev Environment to Cloud (Google / Amazon)
- [ ] Improve Neural Network to overcome Observed Limitations
- [ ] Try Alternative ML methods if needed

## Additional Resources
[Udacity Dataset Torrents](http://academictorrents.com/browse.php?search=Udacity)

