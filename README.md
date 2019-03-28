# deepfake-detector

This project is to develop AI for detecting deepfake videos.

We shall try three pronged approach to detect deepfake videos:
1. Video Signal change detection - QCTools provide various signals which can be used to detect any abnormal change in video.
2. Eye Gesture - Usually eye gesture and lip movement doesn't match completely with lip movement
3. VGG Facial recognition- deepfake can be identified by passing the deepfake video through the VGG trained mode for the given personality which tell the confidence level of deepfake. If confidence levels dropped, it is likely to be deepfake video.
 
Video Signal Detection - A Juypter Notebook is added to generate Video Signals from a file which contains deepfake videos.

Eye Gesture - Orientation of Eye and Eye Blink can be used as metrics along with lip movement.

Eye Blink Detection
https://github.com/m3rc3n4ry/Eye-blink-detection 

Eye Orientation Detection
https://github.com/CSAILVision/GazeCapture

VGG Facial recognition - We believe deepfake videos will show abnormality in facial recognition. This needs to be tested.
https://github.com/serengil/tensorflow-101/blob/master/python/vgg-face.ipynb

Using above three set of features, a composite score for deepfake videos can be developed, which shall be more robust.


