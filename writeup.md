## Project: Search and Sample Return
### Here is writeup written by Ryo Tsutsui.

---


### My github repository:
https://github.com/ryo0221/RoboND-Rover-Project

### Changes
I found this project is very difficult for me, so I bassically followed the guide in the Project Demo Video.

** Rover_Project_Test_Notebook.ipynb **

In the notebook, I added a function to detect rocks, and implemented image_process, as guided in the Demo Video.
The output video file is ./output/my_test_mapping.mp4.


** perception.py **

I implemented perception_step, according to the guidance of the Demo Video.

** decision.py **

I added a mode to approch a rock if there is a rock in the field of view of the rover.
In search mode, Rover steer to the rock and move to it slowly.
When near_sample flag become True and velocity zero, Rover emit send_pickup signal.

### Result
Screen resolution: 1024 x 768
Graphics Quality: Good
FPS: 18

My rover can go around and pick rocks well.
