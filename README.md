# Real Time Exercise Estimation using  Web cam 💪🏋‍♀️

Moto :✍️

The main moto of our project is to count biscep curl based on human pose detection.

Dscription & Working

In this project, we designed poject with  webcam footage to accurately detect exercises in real time and counts reps. OpenCV is used to access the webcam on system, a mediapipe is used to detect body landmarks TensorFlow/Keras to recognize what exercise is being performed.
The detail information for dependencies are provided in requirements.text folder.

Working:👨‍💻

The project is based on Mediapipe Pose detection at the backend which is responsible for calculating the 3D coordinates of the human body keypoints.Then we extract the three: wrist, elbow and shoulder keypoints and form two straight lines joning shoulder and elbow(A) / elbow and wrist(B). Calculating the angle between the two straight lines A and B gives us the angle formed at elbow of the hand which is then used for counter incremnts Working A successful transition of the hand from DOWN to UP increases the counter by 1 each time. Separate counters are maintained for right and left hand.

Thanks for Reading Readme & github page.
