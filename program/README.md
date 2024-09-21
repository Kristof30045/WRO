1. Prototype

   a. **Considerations**  
      - High manoeuvrability  
      - Narrow width  
      - Easy variability of sensor placement  
      - We wanted to build the robot from the Spike kit  
      - Camera (unfortunately this was not available)

   b. **Construction**  
      - Steering gear design with pivot, also known as waist articulation, agreed in advance by e-mail.  
      - Size: 290x100x150 cm  
      - Weight: 605g  
      - Components:  
        - The robot was built from the Lego Spike kit  
        - Lego Spike Brick  
        - Size of the 4 wheels: 56x16mm  
      - Sensors:  
        - 2 distance sensors  
        - 4 axis built-in gyroscope  
        - 1 colour sensor (motor driven by an arm design to identify obstacles to be avoided from above)  
      - Motors:  
        - 3 medium motors:  
          - To rotate the colour sensor  
          - To rotate the steering  
          - To move the robot

 2. Programming
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
