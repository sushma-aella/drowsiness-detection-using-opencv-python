# drowsiness-detection-using-opencv-python

Driver drowsiness detection is a project built using Dlib and OpenCv with Python as a backend language.

OpenCv(opensource computer vision library) is used to detect and recognize faces in this project.
Dlib is used for facial detection and facial landmark detection.
      
# Logic of project

The project includes direct working with the 68 facial landmark detector and also the face detector of the Dlib library.the 68 facial landmark detector is a robustly trained efficient detector which detects the points on the human face using which we determine whether the eyes are open or they are closed.

--shape-predictor : This is the path to dlib’s pre-trained facial landmark detector.
Dlib 68 facelandmark model shows how we can access the face features like eyes,eyebropws,nose,lips etc.





The facial landmarks produced by dlib are an indexable list, as shown here:



![shows-the-face-detection-points-From-the-above-image-the-eyes-are-extracted-by ppm](https://user-images.githubusercontent.com/105199336/170831070-a341d877-a9df-410a-b8f3-63d7ff91dc44.png)



# The working of the project can be found here:


As we can see the above image where the landmarks are detected using the detector.

Now we are taking the ratio which is described as '*Sum of distances of vertical landmarks divided by twice the distance between horizontallandmarks'.

Now this ratio is totally dependent on your system which you may configure accordingly for the thresholds of active,drowsy and sleeping.


![active](https://user-images.githubusercontent.com/105199336/170838879-3c32eedc-21b7-4639-b0e3-0195e7e82cce.png)

![drowsy2](https://user-images.githubusercontent.com/105199336/170839115-facdc74d-8508-4742-bb79-4d61d2f6131b.png)

![sleeping2](https://user-images.githubusercontent.com/105199336/170839358-22bad7dd-6e77-44c0-b380-2b1462151b82.png)

$ python abcd.py \
	--shape_predictor shape_predictor_68_face_landmarks.dat \
