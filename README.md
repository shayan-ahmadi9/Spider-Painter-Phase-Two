# Spider-Painter-Phase-Two

In the first phase, we accomplished a robotic system that could draw a given input on the whiteboard. Although it worked pretty well in the center of the board, It had some setbacks in the corners and the edges of the board. The problem was that in the first phase, we used a set of geometrical equations to define the behavior of each stepper motor in order to steer the robot in a desired trajectory. However, the problem with the corners and the edges was that in those regions, we would face a system of non-linear and complex equations that were not taken into account in the first phase of the project.

In this phase, we would like to correct the parametric and non-parametric errors of the robot by training a neural network. Consequently, the resulting system would be able to follow the desired trajectory with minimum error, regardless of the geometrical orientation of the system. With that intention in mind, we decided to use a smartphone camera to detect the position of the robot and give feedback to the system so that the error decreases.
