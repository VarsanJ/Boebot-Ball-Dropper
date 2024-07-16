# Boebot-Ball-Dropper
This PBASIC program allows a robot to collect a ball at a location using a self-designed 3D printed contraption and drop it in a scoring hole

# Construction and Design
The boebot needs a motor in order to allow another dimension of movement. A servo motor with 270 degrees of rotation was screwed at the front of the boebot using a self-designed motor mount. On the motor, a static arm was attached and a rotating arm was placed in the servo arm so that it rotates when instructed. When everything was screwed in, a counter-weight was attached in the rear of the boebot so that there is counter weight. To improve the movement, two layers of wheel rubber bands were attached on both tires. The rotating arm was also screwed into the mount so that it was more secure. The static arm was a narrower rod whereas the moving arm was wider and longer so that it is better able to hold the rubber ball it collects. A specific design was needed to screw this in and ensure everything fitted. 

# PBASIC code
The code followed the following sequence of steps. 
### (1) Move forward so that it passes the collection holder
### (2) Rotate counter clockwise and move forward towards the collection holder
### (3) Collect the ball by rotating the static arm
### (4) Reverse, rotate and proceed towards the scoring hole
### (5) Push ball into the scoring hole and release the ball
Since the wheels were also motors, movement was controlled by 650 and 850 values. These identified which direction the motor went (clockwise or counterclockwise), impacting how and where the robot moved. After the ball is collected and until it was dropped, the program continued to push the ball into the static arm to prevent it from dropping. This issue was discovered during testing since the ball kept falling out unless the rotating arm kept pushing it. 
The logic I used for the code were iterative structures (for loops) to ensure each of the steps repeated for the needed amount (each pulse of motor)

## Overall Outcome: Ball was able to successfully collect the ball and drop it
