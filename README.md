# KeyStrokes-Dynamics-Based-Authentication-System

User Verification based on Keystroke Dynamics

A program to collect keystroke data, refactor it and analyze it by applying different algorithm model

In Collbration with Urvi Sheth and Aditya Yaji

# Steps to execute
Execute Collecting key stroke.ipynb , enter name, press enter and then enter alphanumeric data on which you want keystroke data. See the stored data in Collecting_keyStroke.csv

After 1, execute calculatingValues.ipynb , this will generate derived values from the previous csv. New Values are stored in, KeyStrokeDistance.csv

execute Analysis.ipynb to see the analysis for both the datasets for the three algorithms mentioned below.

# Proposal
In the project, we will verify the identity of users on the basis of the keystroke information. A model will be first trained by providing it with the typing patterns of the users to be enrolled, multiple patterns per user. The model is then provided with test patterns from the user as well as others posing as that user. The model should be able to reject the imposters while accept the genuine user based on the test pattern similarity to the trained model for the user. We will test various detectors which provide different ways of measuring this similarity. Manhattan Distance Euclidean Distance K-Nearest Neighbours

# Implementation
The implementation for generating key stroke dynamics and model training is done is three phases in this project using python 3.6/3.7:

• Data Acquisition

• Feature Extraction

• Feature Engineering

# Data Acquisition - Datasets
**Dataset 1**
This project mainly uses two datasets, first dataset is collected by running the ipynb named Collecting keystroke. This file takes input from user and stores it into the collecting_keystroke.csv. The first input is the name of the user and after that the user is asked to enter alphanumeric data with some special characters. To get the key stroke dynamics, pyhook python library is used. This library allows to write own event listeners to key up and key down events with the other information such as time, the key id of the key pressed, ascii value of the key pressed etc.

**Dataset -2**
The Second dataset is called CMU Keystroke Dynamics Benchmark Data-set [2] which comprised of keystroke information for 51 users, each user typing the password “.tie5Roanl” 400 times. The recruited 51 subjects (typists) fully completed the study. All subjects typed the same password, and each subject typed the password 400 times over 8 sessions (50 repetitions per session). The password (.tie5Roanl) was chosen to be representative of a strong 10-character password [1].

![image](https://github.com/user-attachments/assets/4717f300-c572-4978-aa3e-8ca84e4bff36)


