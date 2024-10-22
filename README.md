# Deepfake_Video_Detection
Deepfake Video Detection Using RNN

This project focuses on using Python, TensorFlow, and OpenCV to detect deepfake videos with high accuracy. Here’s an overview of the key components and methodologies used in the project:

1. RNN-based Model for Deepfake Detection
   
I built a deepfake detection model using a Recurrent Neural Network (RNN) architecture.

This model achieves 95% accuracy in detecting deepfake videos. RNNs are well-suited for tasks involving sequential data like video, where they can learn patterns over time, which is key for spotting subtle manipulations in fake videos.


2. InceptionV3 for Feature Extraction
   
InceptionV3 was integrated into the system to help extract features from individual frames of the videos.

InceptionV3 is a powerful convolutional neural network typically used in image classification tasks. Here, it helped capture intricate details in each frame, improving the model’s ability to distinguish between real and fake content. This approach led to an average precision of 0.92 and a recall of 0.95, ensuring the model could effectively detect fakes while minimizing false negatives.


3. Preprocessing Using OpenCV

OpenCV was used to handle video preprocessing tasks such as extracting frames and transforming them for model input.

OpenCV efficiently breaks down videos into individual frames, resizes them, and applies any necessary transformations (like normalization). This ensures that each frame is properly formatted for the model, helping improve detection accuracy and model performance overall.


4. Training and Optimization with TensorFlow
   
TensorFlow was used to develop and train the entire deep learning model.

TensorFlow’s framework allowed for easy optimization and deployment of the model. Its flexibility helped in training the RNN-based model efficiently, and it also made it easier to fine-tune parameters for better results. TensorFlow’s scalability means the model can be adapted for real-time video analysis, making it practical for real-world use cases.


5. Robust Performance on Diverse Datasets

The model was rigorously tested on various datasets to ensure its reliability and robustness.

During testing, the model maintained a low false-positive rate (below 3%), which means it rarely misclassified real content as fake. This is crucial in practical applications where high accuracy is needed to prevent false alarms. The model’s performance was consistent across different types of deepfakes, making it a reliable solution for detecting manipulated video
