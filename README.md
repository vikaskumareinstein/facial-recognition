#facial-recognition

In this project we are going to implement face detection and facial recognition on Raspberry pi(3B+,4).
This project is inspired by the facial recognition blog of Adrian Rosebrock.I have implemented some modification and 
included the link to youtube video here.
Raspberry pi 4 for project setup = https://youtu.be/HPQk-gDUrmM<br>
Raspberry pi 3 B+ for project setup = https://youtu.be/P-zxX5KVNBQ<br>
Implementation video of face-detection and recognition = https://youtu.be/Rh830m18dFc<br>

**********************************************************************
For the initial setup of raspberry pi(3/3B+/4) read the `prerequisites.txt` and then install the dependency as written in `dependencies.txt`.After installing all the dependencies run the terminal and put your compressed image(whatsapp compression works better->70-100KB images) in the dataset folder with you name as the name of the folder.

Now run these in your terminal:
  for training on your image-`python encode_faces.py --dataset dataset --encodings encodings.pickle --detection-method hog` using hog detection method.
  for running the script and detecting your image in live video stream -`python pi_face_recognition.py --cascade haarcascade_frontalface_default.xml --encodings encodings.pickle`

Enjoy your face-detection and recognition system.
