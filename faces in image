from cv2 import imread
from cv2 import imshow
from cv2 import waitKey
from cv2 import destroyAllWindows
from cv2 import CascadeClassifier
from cv2 import rectangle


# load the image

pixels = imread('529(2).jpg')
resized_image = cv2.resize(pixels, (1200, 600))

# load the pre-trained model
classifier = CascadeClassifier('haarcascade_frontalface_default.xml')

# perform face detection
bboxes = classifier.detectMultiScale(resized_image, 1.1, 5)

# print bounding box for each detected face
for box in bboxes:
	x, y, width, height = box
	x2, y2 = x + width, y + height
  
	# draw a rectangle over the pixels
	rectangle(resized_image, (x, y), (x2, y2), (0,0,255), 1)
  
# show the image
imshow('face detection', resized_image)

# keep the window open until we press a key
waitKey(0)

# close the window
destroyAllWindows()
