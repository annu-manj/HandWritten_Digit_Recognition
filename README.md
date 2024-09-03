# Digit Recognition using SVM  


This project is focused on digit recognition using Support Vector Machines (SVM). The goal is to classify handwritten digits, which are typically represented as images, into their corresponding numeric labels (0-9). Here's a technical breakdown of how the project is structured:


### Data Preprocessing:  

Standardization: The pixel values of the images are standardized using StandardScaler from sklearn.preprocessing. This process scales the data so that it has a mean of 0 and a standard deviation of 1, which helps the SVM model perform better.  

### Model Construction:

The project uses SVMs for classification, which is a supervised learning method effective for high-dimensional spaces.  
A linear SVM model (model_linear) is trained using a linear kernel, which is suitable when the data is linearly separable.
The model is trained on the standardized training data and then used to predict the labels of the test data.  
RBF Kernel:
A non-linear SVM model (rbf_model) is trained using the Radial Basis Function (RBF) kernel. This kernel is more flexible and can handle cases where the relationship between features is not linear.
Like the linear model, it is trained on the same data and then used to predict test labels.

### Model Evaluation:  

**Accuracy:** The accuracy of both the linear and RBF models is computed using accuracy_score from sklearn.metrics. Accuracy is the ratio of correctly predicted labels to the total number of predictions.  
**Comparison:** The accuracy of both models is compared to understand which kernel performs better on the dataset.  
**Visualization:**
For a visual understanding of the model’s performance, the project randomly selects a few images from the test set, reshapes them to their original 28x28 pixel size, and displays them using matplotlib.
The predicted label from the RBF model is displayed as the title of each image, providing a clear indication of the model's predictions compared to the actual labels.  


