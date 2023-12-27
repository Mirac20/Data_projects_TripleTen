## Project description

The supermarket chain Good Seed would like to explore whether Data Science can help them adhere to alcohol laws by making sure they do not sell alcohol to people underage. We have been given the responsibility of conducting this critical evaluation, guided by the following principles:

1. The stores are equipped with specialized cameras in the checkout zones, activated whenever a purchase of alcohol is detected.
2. State-of-the-art computer vision techniques are employed to ensure an individual's age from a captured photograph.
3. The main objective involves the design, construction, and assessment of a predictive model dedicated to verify a person's age.


To start working on the task, we have a been given a set of photographs of people with their ages indicated.


## Description of the data

- `file_name` - Name of the image
- `real_age` - Age of subject


## **Project Insight**
In this project, I created a model capable of recognizing a person's age through analysis of their pictures. I used the ResNet50 architecture, with a 'relu' activation function to neutralize negative values, and appended an additional terminal layer consisting of a single neuron. This configuration facilitates the production of a solitary output which was derived through regression. The designated loss function was 'mse', and the metric applied was 'mae'. I did not use any form of augmentation in the limitation of training and testing sets. The model's performance reached its peak at a minimum MAE value of 6.45.

