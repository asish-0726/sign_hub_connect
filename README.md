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

  The first phase of the project is dedicated to collecting data for training. The notebook          utilizes the OpenCV library and MediaPipe to detect and draw various landmarks on the human        body (hands, pose, and face).
  
  These landmarks are captured from the webcam and saved as images. These images are later           converted into NumPy arrays for use in training the model.
2. Libraries and Setup:

  Required Libraries:
    cv2: OpenCV for image processing.
    numpy: For numerical operations.
    mediapipe: For landmark detection.
    matplotlib: For visualization purposes.
  The necessary models are loaded via the MediaPipe library, specifically the holistic model      for full-body landmark detection.
