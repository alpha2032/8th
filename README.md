import cv2
Video = cv2.VideoCapture(“video.mp4”)
urrentframe = 0
while(True):
   retrn, frame = video.read()
 if retrn:
   cv2.imwrite(‘img’+str(currentframe)+’.jpg’,frame)
   currentframe += 1
 else:
     break
video.release()
cv2.destroyAllWindows()
