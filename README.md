# VIRTUAL PAINTER #
Step0:
Requirements:
Ubuntu 20.04
webcam
opencv4
g++

Step1:
You need to have several objects which have single and clear color. You will need to
use them as your painters in the next steps.

Step2:
Run the code: 


"""
cd src
export DISPLAY=:0; g++ -o tst1 colorPicker.cpp `pkg-config opencv4 --cflags --libs`
"""


Use your webcam to determine your colors' parameters which is exactly your 


Step3:
Close all windows and end the program run during the Step2.

Step4:
Run:


"""
export DISPLAY=:0; g++ -o tst1 Project1.cpp `pkg-config opencv4 --cflags --libs`
"""
