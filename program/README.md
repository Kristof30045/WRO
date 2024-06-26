# 1. Prototype
a.	Considerations
  i. high manoeuvrability
  ii. narrow width
  iii. easy variability of sensor placement
  iv. we wanted to build the robot from the spike kit
  v.	Camera (unfortunately this was not available)

b.	Construction
  i.	Steering gear design with pivot, also known as waist articulation, agreed in advance by e-mail.
  ii. Size: 290x100x150 cm
  
  iii. Weight: 605g
  
  iv. Components: 
    1. The robot was built from the Lego Spike kit
    2. Lego Spike Brick
    3. size of the 4 wheels: 56x16mm

v.	Sensors: 
  1. 2 distance sensors
  2. 4 axis built-in gyroscope
  3. 1 colour sensor (motor driven by an arm design to identify obstacles to be avoided from above)

vi.	Motors: 3 medium motors:
  1. to rotate the colour sensor 
  2. to rotate the steering
  3. to move the robot

# 2. Programming
a.	Formulation of subtasks
  Straight motion: using gyroscope, we solved the high precision straight motion using P algorithm.
 
  ii. turning: accurate 90° turns are important, so this was dealt with in a separate subtask, also in a separate block (procedure) in the program. 

  iii. from the parking lot: Before exiting the parking lot, distance sensors are used to determine the direction in which the robot will move, and the robot starts the next subroutine accordingly.
  
  iv. to parking: the robot keeps a variable record of the lap it is currently on. After the third lap, it switches to parking mode. It searches for a parking space and performs a partial parking. A separate            block (procedure) is created for this and the turning of the parking spaces is also set in a separate procedure.
      Your block (procedure).

  v.	 Free run task: the procedures tested in the sub-tasks can be combined to solve the Free run task.
       Strategy 1: Maximum speed, maintaining a minimum safe distance from the inner wall. This minimized the running time!
       Test data 2: Average task time: 1 minute 29 seconds


b.	Obstacle course
  i. obstacle detection: 
  1. Obstacle detection is possible with distance sensors facing sideways.
  2. The colour of the obstacle is determined by means of a colour sensor positioned above the sideways projecting obstacle.
  Problem 3: Obstacle detection with high probability of success. Determining the colour of obstacles is successful with low probability.
  Obstacle avoidance: A static sequence of movements can be used to avoid the obstacle and return to the ideal arc. One -one avoidance still has a high probability of success, but many avoidances accumulate         errors and the whole task can get stuck. Thus, we made the strategic decision to maximize points to make sure to finish and park, so we ignored the obstacles and did not touch them. By following the inner arc,    we avoid half of the obstacles from the right direction.  	
