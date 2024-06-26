# Phone Shake Detection problem

The directory contains 3 data sets. 

1) a.lbl.csv a.sensor.csv
2) m.lbl.csv m.sensor.csv
3) p.lbl.csv p.sensor.csv

Each set has two files sensor.csv wnd lbl.csv. 

The sensor.csv has data from various phone sensors. Here is description of various columns. 

timestamp(ms)  : Unix Timestamp in milliseconds.
acceleration_x(g) : Acceleration along phone's x axis (measured in g)
acceleration_y(g) : Acceleration along phone's y axis (measured in g)
acceleration_z(g) : Acceleration along phone's z axis (measured in g)
roll(rad) : Roll angle representing phone's attitude (orientation)
pitch(rad) : Pitch angle representing phone's attitude (orientation) 
yaw(rad) : Yaw angle representing phone's attitude (orientation)
angular_velocity_x(rad/sec) : Angular velocity around x axis (passing thru phones center along smaller edge)
angular_velocity_y(rad/sec) : Angular velocity around y axis (passing thru phones center along longer edge)
angular_velocity_z(rad/sec) : Angular velocity around z axis (passing thru phones center emerging out of phone )

The data is recorded every 100 ms (10Hz frequency). 

The second file lbl.csv contains 3 types of labels 

1) Label 0 : Represents start of Shake gesture 
2) Label 1 : Indicates end of Shake gesture

The Goal of the exercise is to create a classifier that can be implemented easily on streaming sensor data to detect Shake gesture. 