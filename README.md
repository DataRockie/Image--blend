# Image-blend
Image blend merges two photographs of different people in the same background to create a single multi person blended photograph.
The input to the program is the two images of different people front facing and the output is one single blend image.
It uses ORB (Oriented FAST and Rotated BREIF) descripter to find the the interest points in the input images. Then keypoints matching is done to estimate homography to wrap one of the image so that the perpective of two image must be same in order to blend the images. 
Locating the subjects in the pictures is important for determining which image merging process to use.To detect the face of the person in the image  Haar Feature-based Cascade Classifiers is used and based oh the detected coordinates(x,y) the body of the person is detected .
Alpha blending technique is used to blend the first image with the wrapped second image.


