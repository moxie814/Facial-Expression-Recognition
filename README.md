# Facial-Expression-Recognition
Detects the face expression and labels it with the suitable expression name using DeepFace Library


# Overview

The real-time facial emotion recognition project utilizes Python along with OpenCV and DeepFace libraries to detect and analyze emotions in live webcam feeds. It employs a face cascade classifier to detect faces in each frame captured from the webcam. Once faces are detected, the DeepFace library is utilized to analyze the emotions present in the detected faces. 


Used:
1.Python: Programming language used for development. <br>
2.OpenCV (cv2): Library for computer vision tasks such as image and video processing.<br>
3.DeepFace: Library for facial analysis, including emotion detection.<br>


# Working
1. Initialization:
The code initializes the OpenCV library (`cv2`) for computer vision tasks and imports the `DeepFace` library for facial analysis.
2. Face Cascade Classifier:
 It loads a pre-trained face cascade classifier (`haarcascade_frontalface_default.xml`) provided by OpenCV. This classifier is used to detect faces in the webcam frames.
3. Video Capture:
 The code starts capturing live video frames from the default webcam (`VideoCapture(0)`).
4. Face Detection:
  For each frame captured by the webcam, the code detects faces using the face cascade classifier's `detectMultiScale` method. This method returns the coordinates of bounding boxes around detected faces.
5. Emotion Analysis:
  Once a face is detected, the code extracts the region of interest (ROI), i.e., the detected face, from the frame.
6. Visualization:
After analyzing the face, the code draws a rectangle around the detected face and labels it with the predicted emotion. 
7. Real-time Display:
The resulting frame, with bounding boxes and emotion labels, is continuously displayed in real-time using `cv2.imshow`.
8. Loop and Exit Condition:
The entire process is executed in a loop, allowing for continuous real-time analysis of the webcam feed.
9. Resource Release:
Once the program is terminated, the video capture object is released (`cap.release()`), and all OpenCV windows are closed (`cv2.destroyAllWindows()`).
![image](https://github.com/moxie814/Facial-Expression-Recognition/assets/148361595/d3de5c96-9427-4db6-92ee-9c037f4834eb)

