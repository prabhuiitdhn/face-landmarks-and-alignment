This is for using the dlib library which detects the facial landmarks and alignment of faces using helendataset.

For dlib library please follow the following steps to install in Linux system.
>> $ sudo apt-get install build-essential cmake
>> $ sudo apt-get install libgtk-3-dev
>> $ sudo apt-get install libboost-all-dev

If you haven't install the pip follwo the following steps to install pip

>> $ wget https://bootstrap.pypa.io/get-pip.py
>> $ sudo python get-pip.py

Open your bash profile
>>$ nano ~/.bash_profile
>># Homebrew
  export PATH=/usr/local/bin:$PATH
  
>>$ source ~/.bash_profile

Install python and python 3 
>>$ brew install python
>>$ brew install python3
>>$ brew install cmake
>>$ brew install boost
>>$ brew install boost-python --with-python3

As a sanity check, I would suggest validating that you have both boost  and boost-python  installed before proceeding:

How to install dlibShell

As a sanity check, I would suggest validating that you have both boost  and boost-python  installed before proceeding:
$ brew list | grep 'boost'
boost
boost-python

Install python binding
>>$ pip install numpy
>>$ pip install scipy
>>$ pip install scikit-image
>>$ pip install dlib

Now you've successfully install dlib for checking in your system
>>python
>>import dlib //if this is not giving ny error that means congrats, you've successfully installed dlib for face landmarks and face allignments.

Understanding the face 

Understanding dlib’s facial landmark detector:
The pre-trained facial landmark detector inside the dlib library is used to estimate the location of 68 (x, y)-coordinates that map to facial structures on the face.

For running the program 
Please install/ upgrade your imutils package using pip install --upgrade imutils

For face_landmark.py

parse our command line arguments:

--shape-predictor : This is the path to dlib’s pre-trained facial landmark detector. You can download the detector model here or you can use the “Downloads” section of this post to grab the code + example images + pre-trained detector as well.
--image : The path to the input image that we want to detect facial landmarks on.

Download the shape_predictor 
http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2


  


