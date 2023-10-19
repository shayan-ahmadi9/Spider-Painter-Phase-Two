# Spider-Painter-Phase-Two

*Note: The details on the first phase of this project can be found at: https://github.com/shayan-ahmadi9/Spider-Painter-Phase-One

In the first phase, we accomplished a robotic system that could draw a given input on the whiteboard. Although it worked pretty well in the center of the board, It had some setbacks in the corners and the edges of the board. The problem was that in the first phase, we used a set of geometrical equations to define the behavior of each stepper motor in order to steer the robot in a desired trajectory. However, the problem with the corners and the edges was that in those regions, we would face a system of non-linear and complex equations that were not taken into account in the first phase of the project.

In this phase, we would like to correct the parametric and non-parametric errors of the robot by training a neural network. Consequently, the resulting system would be able to follow the desired trajectory with minimum error, regardless of the geometrical orientation of the system. With that intention in mind, we decided to use a smartphone camera to detect the position of the robot and give feedback to the system so that the error decreases.

In the beginning, we decided to find out our detection error before going any further. To do so, the detection of a number of various points from different distances and different angles was carried out. Overall, the mean square error over 1152 detected points, was about 1 cm. As a result, we needed to improve the accuracy of the detection.

In order to improve the detection accuracy, we trained an MLP model. With the help of this model, the root mean square error of the detection reached the value of about 0.46 cm, which demonstrates a major improvement in the accuracy of detection.

Our next goal is to make use of this accurate detection system, as a sensor in a feedback system to control the position of the robot.
