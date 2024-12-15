# sign_hub_connect
This is a Machine Learning Model Integrated with website which can converts sign language to text.

Hi Everyone my name is Asish. Me and my team has built an LSTM model integrated with website that converts sign language to text. 
Lets dive deep to this Project.

This project is Divided into 3 parts 
1. Data Collection Part
2. Preprocessing Part
3. Real Time Deployment Part

Now lets talk about Data Collection Part 

DATA COLLECTION PART 
1.Data Collection:
The first phase of the project is dedicated to collecting data for training. The notebook utilizes the OpenCV library and MediaPipe to detect and draw various landmarks on the human body (hands, pose, and face).These landmarks are captured from the webcam and saved as images. These images are laterconverted into NumPy arrays for use in training the model.

2. Libraries and Setup:
   Required Libraries:
   1. cv2: OpenCV for image processing.
   2. numpy: For numerical operations.
   3. mediapipe: For landmark detection.
   4. matplotlib: For visualization purposes.
The necessary models are loaded via the MediaPipe library, specifically the holistic model for full-body landmark detection.
Functions:

mediapipe_detection: Converts the image to RGB, runs it through the MediaPipe model, and converts it back to BGR.
draw_landmarks: Draws the detected landmarks for the face, hands, and body pose on the image.
Key Steps:
Initialization:
The holistic model is set up for detecting facial, hand, and pose landmarks.
Functions for detecting and drawing landmarks are defined.
Real-time Data Collection:

The code continuously captures frames from the webcam.
Detected landmarks are drawn on each frame, and the images are saved to a designated directory.
Important Points:
The dataset is being built using hand, pose, and face landmarks from the MediaPipe library.
The collected data is stored in NumPy array format for later use in model training.
Real-time application: This script can be used in real-time applications to collect landmarks for further model training or deployment.


