# Predicting Funding Success: Neural Network Model for Alphabet Soup
Overview of the Analysis

Alphabet Soup aims to efficiently allocate funding to applicants with the highest likelihood of success. By leveraging machine learning and deep learning, this analysis builds a binary classifier using a neural network model to predict whether an applicant will successfully utilize the funding.

Results

Data Preprocessing
- Target Variable: IS_SUCCESSFUL (binary indicator of funding success)
- Feature Variables: Application metadata (e.g., APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, etc.)
- Removed Variables: EIN and NAME, as they are unique identifiers and do not contribute to the predictive analysis.

Compiling, Training, and Evaluating the Model
- Number of Layers & Neurons:
- First Hidden Layer: 64 neurons, ReLU activation
- Second Hidden Layer: 32 neurons, ReLU activation
- Output Layer: 1 neuron, Sigmoid activation
- Optimization Choices:
- Binary cross-entropy loss function (suitable for classification)
- Adam optimizer (adaptive learning rate)
- Model Performance:
- Loss: 0.5632
- Accuracy: 72.52%
- Optimization Steps Taken:
- Feature Scaling: Standardized numerical values
- Categorical Encoding: Converted text data via one-hot encoding
- Hyperparameter Tuning: Adjusted neuron count and activation functions

Summary & Recommendations

The model achieves 72.52% accuracy, slightly below the 75% target. Several strategies can optimize performance further:
- Increasing Hidden Layers: A deeper network might extract more complex patterns.
- Testing Alternative Activation Functions: Leaky ReLU or tanh may improve convergence.
- Experimenting with Different Models:
- Random Forests (better feature importance evaluation)
- Gradient Boosting (stronger predictive power for classification)

Conclusion

While the neural network provides reasonable accuracy, additional refinements and alternative models may yield better results for Alphabet Soup’s decision-making process.
