# Supermarket Age Recognition Model

**Project Description**: <br> The supermarket chain Good Seed is interested in exploring a Data Science approach to help with customer age recognition in order to aid with the sales of alcohol legally. The customer's photo will be taken at the checkout area if they scan an alcoholic beverage and computer vision methods should be used to determine the age ofa person from that photo. The goal of this project will be to create a model for verifying people’s ages. 

**Dataset**: <br> A dataset. faces.csv of 7591 images, was provided containing photos of peoples and their real ages.

**Exploratory Data Analysis (EDA):** <br>
1. Plotted histogram of Age Distribution 
2. Data Augmentation, images were rotated and converted to grayscale 

**Model Development:** <br>
The age recognition model is built using a ResNet50 architecture with a custom head. The model is trained using the Adam optimizer with a learning rate of 0.0005 and mean squared error (MSE) as the loss function. We split the dataset 80/20 with 80 percent of the data reserved for training. The train_model function trains the model using the training set and validates with the validation set. To prepare the script for running on the GPU platform, we define the necessary functions and combine them into a single script. 

**Results:** <br> 
The model has achieved an MAE of 7.6512 on the validation set, which meets the project criteria of MAE not higher than 8. 

**Conclusion:** <br>  The MAE score for the model decreases as the epochs increase meaning it is getting better at making accurate predications about people’s ages and is generalizing well which is important because the model is expected to take in new data constantly. This is a good sign that Good Seed can employ such method. For future, the model can be better improved by hyperparameter tuning and ensuring that data being fed is diverse in demographics to ensure there won't be a biased. 






