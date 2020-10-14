# realtime face recognition with deep learning in python

The code of a project about using deep-learning to realize the face recognition in my project group(4 people).

The detection of face is using OPENCV.

We need to prepare at least 5 photos of every person in the project (in this example so totally 5*4=20 photos) and then we use baseofimage.py to transform each photo randomly into 100 different photos, so totally 500 photos for each person. Then take the face part of each transformed photo, and apply LBP to them and save the new photos in the folder CNNdata.(You can change the path in the python code (baseofimage.py)as you want.)

Then we have totally 2000 images after LBP for training the model. Use train.py to train the model and the trained model is saved as model.h5 and model.json.

Phototest.py is for testing the face recognition between our 4 people by the photos. We prepared some other photos or the test.

Load.py is consisted by 3 parts. Print the accuracy by the test of random 10% images of CNNdata. Print the result of 5 special photos choosen from CNNData folder.(The fifth photo is by a person out of our group) And the real-time face recognition with a webcamara.

All the third party packages we used is here(with python2): keras,cv2,numpy,skimage,sklearn,tensorflow(ver.1.0.0+)

PS: The final step of my project is realized by Raspberry PI 3 and PI camera. We trained the model with a computer (with or without GPU) and then move all the necessary files into Raspberry PI. If you have the same devices (I mean the raspberry pi and pi camera), you can also try to use my load_pi.py to do the realtime face recognition on raspberry pi.

Here is a video that I made to show you the result that I got.  https://www.youtube.com/watch?v=rY_uSFl2TcA&feature=youtu.be

You shoud made a modified version of this code
