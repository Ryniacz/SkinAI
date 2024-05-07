SkinAI is an advanced AI system designed for the automated evaluation of dermatological images to identify a range of skin conditions. This tool is intended to enhance the speed and accuracy of diagnosing skin diseases, supporting dermatologists and enhancing access to high-quality skin care.

Programming Environment: Python Key Libraries: TensorFlow, Keras, NumPy, Matplotlib, scikit-learn Functionality: Employs a Convolutional Neural Network (CNN) for the classification of skin conditions. Input: A dataset of labeled skin images. Output: Outputs model accuracy evaluation, a confusion matrix, a comprehensive classification report, visual representations of model accuracy and loss, and sample image predictions.

Script Workflow:

Model Loading: Begins by loading a pre-trained model equipped with the best weights from previous validation efforts.

Model Evaluation: Evaluates the model with a test dataset to determine loss and accuracy, which are then displayed.

Predictions: Outputs predictions for the test dataset, categorizing each image under the most probable disease classification.

True Labels Preparation: Creates a vector of actual labels from the test dataset for accuracy assessment.

Training History Visualization: Displays charts of training and validation accuracy and loss through time to illustrate the model’s learning curve.

Confusion Matrix: Compiles and exhibits a confusion matrix to visually indicate the model's performance in differentiating among various diseases.

Classification Report: Generates a detailed report with precision, recall, and F1 scores for each disease category, showcasing the model’s classification capabilities.

Sample Predictions Display: Demonstrates a series of five test images along with their actual and predicted labels to highlight the model’s diagnostic proficiency.