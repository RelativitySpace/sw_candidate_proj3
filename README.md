# Background

You have joined Relativity Space's mission of building rockets in less than 60 days and have been tasked with building the end to end software for 3D printing rockets autonomously. 

In its roots, as depicted in the diagram below, this system comprises of a robot whose end effector is fitted with multiple sensors and a welder that deposits metal along the path that the robot has been commanded to follow. To correct for any errors along the path, a closed loop controller receives feedback from the sensors and adjusts the robot's position accordingly.

![alt text](images/welding-robot.JPG?raw=true "Robotic Welding System")

# Homework Assignment

The robotic welding system shown above encounters errors along the Y axis that need to be corrected for, based on information received by the sensor that is mounted onto the arm.

Simulate an environment with the following:
- Robot: That receives move commands to be executed at 1Hz but randomly misses the target location
- Sensors: You can choose any number of sensors and use any mathematical functions to simulate the data sent by the sensor	
- Closed loop controller: That sends move commands to the robot and receives sensor inputs that can be used for correcting the path
	
The following requirements need to be met with:
- Provide a graphical user interface that can be used to turn the sensors on or off
- Store the sensor data in a time series database (E.g. Prometheus, InfluxDB)
- Use a monitoring tool to visualize the data in real-time (E.g. Grafana, Kibana)

Your work will be evaluated based on how deep into the optional requirements you go:
- Build out the sensors and the controller as separate processes that can communicate with each other
- Monitor the error along the Y axis in the simulated robot, in real-time
- Add an additional feature to the user interface that can be used to turn the controller on or off without breaking the system

You can use any programming language, operating system and off the shelf libraries to build this system out.

Submission instructions:

- Commit your code to a public Github repository
- Include a software design diagram
- Include installation instructions
- Email the link to your repository to our recruiter at least a day before the review call 

Please do not fork this repository.


