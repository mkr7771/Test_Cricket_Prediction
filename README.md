# Test_Cricket_Prediction
Test Cricket Prediction using Inverse Reinforcement Training Model

Project Overview:
In this project, I developed a system for predicting cricket match outcomes using Inverse Reinforcement Learning (IRL). IRL is a machine learning technique that learns from expert demonstrations to infer the underlying reward function. The goal was to predict various match actions such as batting and bowling decisions based on match state features.

Key Steps:

Data Collection and Preprocessing:

Acquired a dataset containing cricket match data, including features such as inning, overs, cumulative total runs, team names (bat_team and bowl_team), runs scored, wickets taken, and ball number.
Preprocessed the data by converting categorical variables (team names) into numerical values using a dictionary mapping.
Split the dataset into training and testing sets for model training and evaluation.
Model Definition:

Defined a Maximum Entropy Inverse Reinforcement Learning (MaxEnt IRL) model using PyTorch.
The model architecture consisted of a linear layer to map input features (match state) to predicted rewards (actions).
Model Training:

Trained the MaxEnt IRL model using the training dataset.
The model learned to predict expert actions (batting and bowling decisions) based on input match state features.
Training involved optimizing model parameters to minimize the Mean Squared Error (MSE) loss between predicted and expert actions.
Model Evaluation:

Evaluated the performance of the trained model on the test dataset.
Calculated the average loss (MSE) on the test data to assess the model's accuracy in predicting cricket match actions.
Model Saving and Loading:

Saved the trained model to a file using PyTorch's torch.save method for future reuse without retraining.
Prediction and Post-processing:

Used the trained model to make predictions on new data, representing match state features.
Performed post-processing on predicted action values to ensure they followed predefined rules.
Validated and adjusted predicted actions to ensure consistency and adherence to cricket match rules.
Result Analysis:

Analyzed the predicted results to determine the winning team, calculate total scores for each team, and compute the lead by score.
Provided insights into the outcome of the simulated cricket match based on predicted actions.
Conclusion:
This project showcased the implementation of Inverse Reinforcement Learning techniques for cricket match prediction. By leveraging expert demonstrations and machine learning algorithms, the system demonstrated the ability to predict match outcomes and provide valuable insights into cricket match dynamics.
