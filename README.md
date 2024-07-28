## Hand Gesture Recognition Model for Intuitive Human-Computer Interaction

**Objective:**
To develop a hand gesture recognition model that can accurately identify and classify different hand gestures from image or video data, enabling intuitive human-computer interaction and gesture-based control systems.

**Description:**
This project aims to create a robust hand gesture recognition system using deep learning techniques. The model is designed to classify various hand gestures, facilitating natural and intuitive interaction between humans and computers.

**Steps Involved:**

1. **Data Collection:**
   - Images of different hand gestures were collected and organized into subdirectories, each representing a different gesture class.

2. **Data Loading:**
   - Images were loaded from the dataset directory using OpenCV. Each image was read and appended to a list along with its corresponding label.

3. **Data Preprocessing:**
   - Loaded images were converted into numpy arrays and normalized by scaling pixel values between 0 and 1.
   - Labels were encoded into numerical values using `LabelEncoder`.
   - The dataset was split into training and testing sets with a 70-30 ratio to ensure a balanced evaluation.

4. **Model Architecture:**
   - A Convolutional Neural Network (CNN) was constructed using TensorFlow's Keras API.
   - The network consists of multiple convolutional layers followed by max-pooling layers, which help in extracting spatial features from the images.
   - The final layers included a flattening layer, a dense layer with ReLU activation, and an output layer with softmax activation to classify the gestures.

5. **Model Training:**
   - The model was compiled using the Adam optimizer and sparse categorical cross-entropy loss.
   - Training was conducted over 10 epochs with a batch size of 32. The model was validated on the test set after each epoch.

6. **Model Evaluation:**
   - The trained model achieved a remarkable accuracy of 100% on both the training and validation sets.
   - The test set evaluation confirmed the model's accuracy at 100%, demonstrating its ability to generalize well to unseen data.

**Conclusion:**
The hand gesture recognition model successfully classifies different hand gestures with high accuracy, making it a reliable tool for gesture-based control systems and intuitive human-computer interaction. Future work could involve expanding the dataset to include more gestures and testing the model in real-time video streams to further enhance its applicability.

**Dataset Link -** https://www.kaggle.com/datasets/gti-upm/leapgestrecog
