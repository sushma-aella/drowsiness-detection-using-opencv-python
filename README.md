# drowsiness-detection-using-opencv-python

Driver drowsiness detection is a project built using Dlib and OpenCv with Python as a backend language.

OpenCv(opensource computer vision library) is used to detect and recognize faces in this project.
Dlib is used for facial detection and facial landmark detection.
      
# Logic of project

The project includes direct working with the 68 facial landmark detector and also the face detector of the Dlib library.the 68 facial landmark detector is a robustly trained efficient detector which detects the points on the human face using which we determine whether the eyes are open or they are closed.

--shape-predictor : This is the path to dlib’s pre-trained facial landmark detector.
Dlib 68 facelandmark model shows how we can access the face features likeeyes,eyebropws,nose,lips etc.














$ python abcd.py \
	--shape_predictor shape_predictor_68_face_landmarks.dat \
