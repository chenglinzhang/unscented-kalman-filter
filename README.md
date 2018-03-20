## 2. Unscented Kalman Filter Project

### Self-Driving Car Engineer Nanodegree Program - Term 2

This project utilizes an Unscented Kalman Filter to estimate the state of a moving object of interest with noisy lidar and radar measurements. 

[//]: # (Image References)
[image1]: ./images/screenshot.png

This project involves the Term 2 Simulator which can be downloaded [here](https://github.com/udacity/self-driving-car-sim/releases)

INPUT: values provided by the simulator to the c++ program

```
["sensor_measurement"] => the measurment that the simulator observed (either lidar or radar)
```

OUTPUT: values provided by the c++ program to the simulator
```
["estimate_x"] <= kalman filter estimated position x
["estimate_y"] <= kalman filter estimated position y
["rmse_x"]
["rmse_y"]
["rmse_vx"]
["rmse_vy"]
```

The result looks like the following on the simulator:

![alt text][image1]

### Other Important Dependencies
* cmake >= 3.5
  * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1 (Linux, Mac), 3.81 (Windows)
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools](https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)

### Basic Build Instructions

1. Clone this repo.
2. Make a build directory: `mkdir build && cd build`
3. Compile: `cmake .. && make`
4. Run it: `./UnscentedKF` Previous versions use i/o from text files.  The current state uses i/o
from the simulator.

### Code Style

Follow [Google's C++ style guide](https://google.github.io/styleguide/cppguide.html) as much as possible.

