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

