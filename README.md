SkinAI is an advanced system based on artificial intelligence, designed for the automatic analysis of skin images to detect and diagnose various skin diseases. Its aim is to provide a quick, accurate, and efficient method of diagnosing skin diseases to support dermatologists and enhance access to high-quality dermatological care.

Programming Language: Python
Libraries: TensorFlow, Keras, NumPy, Matplotlib, scikit-learn
Function: Classification of skin diseases using a Convolutional Neural Network (CNN)
Input: Labeled dataset of skin images
Output: Model accuracy assessment, confusion matrix, classification report, accuracy and loss visualizations, and sample images with predictions
Script Operation Description:

Model Loading: The script begins by loading trained model weights that have performed best on validation data.

Model Evaluation: The model is evaluated on the test dataset, and the results (loss and accuracy) are displayed on the console.

Predictions: It makes predictions on the test set, then assigns the most probable class for each test image.

True Labels: The script prepares a vector of true labels using data from the test generator.

Training History Visualization: Displays plots of accuracy and loss for the training and validation data, which helps assess how the model learned over time.

Confusion Matrix: Creates and displays a confusion matrix, which is a graphical representation of the classification outcomes. It is useful for understanding which classes are confused by the model.

Classification Report: The script generates a classification report that includes metrics such as precision, recall, and F1 score for each class.

Sample Predictions: At the end, it displays five examples of test images along with their true and predicted labels, providing insight into the model's performance.

Note that the above script must be run in an environment where the appropriate libraries are already installed and configured, and that the data must be pre-processed and divided into training, validation, and test sets. The script also assumes that the dataset is balanced and properly labeled, and that images are scaled to a uniform size.