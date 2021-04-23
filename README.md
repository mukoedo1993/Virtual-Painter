# VIRTUAL PAINTER #
It is an implementation of a virtual painter based on C++ and Opencv library.
Reference:
https://www.youtube.com/watch?v=2FYm3GOonhk

# STEPS #
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
```
cd src
export DISPLAY=:0; g++ -o tst1 colorPicker.cpp `pkg-config opencv4 --cflags --libs`
./tst1
```
Use your webcam to determine your colors' parameters which is exactly your painter's color.
Adjust your scrollwindow's parameters.
See:
![mask](Image_mask.png)
And the trackbar:
![mask](trackbar.png)

Step3:
Close all windows and end the program run during the Step2.

Step4:
Adjust line18 to line 23's code of Project1.cpp, using parameters obtained from Step2.
```
//adjust your painter's hue, saturation and val values one by one.
vector<vector<int>>myColors {//{15,23,166,255,91,124},//a yellow brush
                             {0,169,139,10,255,255,255},//a pink pencil
                             {139,55,135,179,123,188}  //a purple pencil(DOEN'T WORK WELL)
                            };

vector<Scalar>myColorValues{
                            {0, 0, 139},//dark blue
                            {255, 192, 203},//pink 
                            //

};
```

Step5:
Run:
```
export DISPLAY=:0; g++ -o tst1 Project1.cpp `pkg-config opencv4 --cflags --libs`
./tst1

```
See the image:
![painted_image](painted.png)

Admittedly, my painter and webcam are very poor... :)
