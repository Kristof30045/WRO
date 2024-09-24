# 1. Programming

   ## a. Formulation of Subtasks
   1. **Straight motion:** Using the gyroscope, we solved the high precision straight motion using the P algorithm.
   
   2. **Turning:** Accurate 90° turns are important, so this was dealt with in a separate subtask, also in a separate block (procedure) in the program.
   
   3. **From the parking lot:** Before exiting the parking lot, distance sensors are used to determine the direction in which the robot will move, and the robot starts the next subroutine accordingly.
   
   4. **To parking:** The robot keeps a variable record of the lap it is currently on. After the third lap, it switches to parking mode. It searches for a parking space and performs a partial parking. A separate block (procedure) is created for this, and the turning of the parking spaces is also set in a separate procedure.
   
   5. **Free run task:** The procedures tested in the subtasks can be combined to solve the free run task.  
      - **Strategy 1:** Maximum speed, maintaining a minimum safe distance from the inner wall. This minimized the running time!  
      - **Test data:** Average task time: 0 minute 55 seconds.

# Main flowchart for Open challange
![flowchart](Openflowchart.jpg)


## b. Obstacle Detection

A machine learning add-on is available for the LEGO MINDSTORMS Robot Inventor software, allowing users to integrate machine learning models into their robots. This add-on typically includes the following:

<img src="../pictures/obstacle.jpg" alt="maching learning" width="500">


1. **Image Data Processing:** The add-on enables the use of the phone camera's image and utilizes this data for training machine learning models. It often includes predefined models that help users quickly start machine learning projects. These models typically address fundamental tasks such as image recognition or identifying movement patterns.

2. **Training:** We train four models (Right Red Obstacle, Left Red Obstacle, Right Green Obstacle, Left Green Obstacle). Eight to ten photos per model are sufficient.

3. **Usage:** When the robot is in front of the obstacle, it uses the machine learning add-on. It moves according to the most likely option provided by the four models.

<img src="../pictures/machinglearning.jpg" alt="maching learning" width="300">

# Main flowchart for Obstacle challange
![flowchart](Obstacleflowchart.jpg)


# 2. Block code
![code 1](code1.jpg)
![code 2](code2.jpg)


# Hardware:
This project can be done with a laptop or a computer running windows 10 or newer if you can connect the hub with a data 
cable or bluetooth to the computer/laptop, a mobile phone that support the mindstorms app and have the necessary softwares


# Softwares for programming the Spike hub:

We first used the Lego Spike desktop application which can be downloaded from the Lego Educations website 

![spike_donwload](https://github.com/user-attachments/assets/0c583583-927f-476d-be77-bc5f6d7d77c6)

And we used an online editor that can be opened in a browser that supports connecting to the hub (we used Google Chrome)

We could not complete the obstacle challange with the Spike because we did not had a camera so we only focused on the open challange and make it
as good as possible.


# Software for programming the Mindstorms hub:

We used the official Mindstorms app(we downloaded it from microsoft store)

<img src="mindstorms.png" alt="mindstorms">


Fortunately we did not needed any downloadable extensions because the mindorms app supports machine learning and we used that
to indentify any obstacle (you can apply it when you open block extensions in the bottom left corner and in the experimental 
section enable machine learning)

<img src="block_extensions.png" alt="block extensions">

![extensions2](https://github.com/user-attachments/assets/bafc4e21-3fd3-49a3-be0b-c926aeccb9cd)
![sensors](https://github.com/user-attachments/assets/19844584-cdb9-4b06-b388-53936e935848)

<img src="machine_learning_on.png" alt="machine learning enable">

For this we used a mobile phone that supported the Lego Mindstorms app uploaded the code 
to the phone and we trained the AI to indentify the obstacles and which side is it at(left or right)

<img src="../pictures/obstacle.jpg" alt="training the AI">



# The open challange with comments:

![fo_program2](https://github.com/user-attachments/assets/41bdce33-ba3e-4098-9a56-8c4aefa31949)
![kiparkolas_beparkolas2](https://github.com/user-attachments/assets/bf806642-59da-4397-9a35-42f1b21b9d79)
![jobb_bal2](https://github.com/user-attachments/assets/cb149c49-aff6-4655-b09b-e49971e9849d)
![fok-kez_kor-szaml2](https://github.com/user-attachments/assets/94cb21c5-37a6-4b8c-a99c-82255d899d1a)
![egyenes_p2](https://github.com/user-attachments/assets/c2e26206-28fa-4087-b36a-87a94dedbe95)
![90fok2](https://github.com/user-attachments/assets/981b67cb-e153-43e3-9dea-b65437d518d5)

# The obstacle challange with comments


![fo_program](https://github.com/user-attachments/assets/e0e69169-46ca-4a9c-93d7-29b3e5d37507)
![kerules_eldontes](https://github.com/user-attachments/assets/416b93fc-960e-4d28-95ae-b3365371232b)
![ki-be_parkolas](https://github.com/user-attachments/assets/55d14ac1-c6b7-4a79-8557-17d857f77f3f)
![kerulesek jpg](https://github.com/user-attachments/assets/1a30e898-3969-46d0-9255-66c9f1bed4ee)
![pontos_kanyar](https://github.com/user-attachments/assets/32a0676c-2473-49f3-aab7-3afb79ccae46)
![fok_kez-kor_szaml](https://github.com/user-attachments/assets/87aed081-79d4-4cf1-bffc-6b8cf42f2850)
![egyenes_p](https://github.com/user-attachments/assets/7e0fd1b8-1120-40dd-a979-71b6f83b23f5)

