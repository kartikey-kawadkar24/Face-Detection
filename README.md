Face detection project is mainly used to see how does the HaarCascadeClassifier works.
Detecting faces in an image can give us the count of people present in an image and if
all the faces are possibly being able to be detected or not.

So, in this project we have used OpenCV library to read the image and classifier to 
detect faces using "Scale Factor" which helps in finding and detecting small faces in
a large sized image by rescaling it by a small step. You can find the detailed code in
"faces in image.py" file provided.

A similar approach can be used to detect the faces in real time, the way our mobile 
phones does after switching on the camera. This is mainly used to get a proper focus
on all the faces present in the frame without distorting any or considering any face
as background. This level of accuracy is achieved using "MinNeighbors" parameter which
tells us how many neighbors each candidate rectangle should have to detect it as a face.
So, it detects the face based on neighboring candidates. You can find the detailed code
in "faces in real time.py" file provided.
