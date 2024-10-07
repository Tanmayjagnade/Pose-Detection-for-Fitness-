# Real Time Exercise Detection using  Web cam 💪🏋‍♀️

## Moto :✍️

The main objective of this project is to design and implement a Convolutional Neural Network (CNN) along with pretrained (MediaPipe) models capable of detecting a person's posture and repetitions accurately
Created a user-friendly interface with real-time feedback on posture correctness using Python, OpenCV, MediaPipe, and TensorFlow/Keras.

##Components*

- *Webcam Integration*: Utilizes OpenCV for real-time video capture.
- *Exercise Detection*: Implements deep learning models using TensorFlow/Keras.
- *Posture Assessment*: Analyzes posture correctness using MediaPipe.
- *User Interface*: Built using Python for easy navigation.


*Usage*

1. Run the application.
2. Perform bicep curls in front of the webcam.
3. Receive real-time feedback on posture correctness.
4. View exercise tracking and counting on the interface.

*Dependencies*

- Python
- OpenCV
- MediaPipe
- TensorFlow/Keras


*How to Use*

1. Clone the repository.
2. Install required dependencies using pip install -r requirements.txt.
3. Run the application using python (link unavailable)
4. Access the application through a web browser at http://localhost:5000
5. Installing the depedencies:

pip install requirements.txt

Separate counts will be recoreded for left and right bicep curls. Press 'r' key to reset the counter anytime and 'Esc' to quit. To run the app, execute the following on the terminal:

python demo.py

## Dscription & Working:

In this project, we designed project with webcam footage to accurately detect exercises in real time and counts reps. OpenCV is used to access the webcam on system, a mediapipe is used to detect body landmarks TensorFlow/Keras to recognize what exercise is being performed. The detail information for dependencies are provided in requirements.text folder.

## Working:👨‍💻

The project is based on Mediapipe Pose detection at the backend which is responsible for calculating the 3D coordinates of the human body keypoints.Then we extract the three: wrist, elbow and shoulder keypoints and form two straight lines joning shoulder and elbow(A) / elbow and wrist(B). Calculating the angle between the two straight lines A and B gives us the angle formed at elbow of the hand which is then used for counter increments Working A successful transition of the hand from DOWN to UP increases the counter by 1 each time. Separate counters are maintained for right and left hand.

## References

Guide to Human Pose Estimation with Deep Learning(Nanonets)

Mediapipe Pose Classification(Google's Github)

(AI Pose Estimation with Python and MediaPipe)

Thanks for Reading Readme & github page.
