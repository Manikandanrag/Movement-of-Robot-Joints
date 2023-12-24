# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```
Developed by: Manikandan R
RegisterNumber: 23004754
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
  pos=[[1,30],[2,40],[3,90]]
  robot = getRobot()
  robot.driveJoints(0,0,0,0,0,0)
  delay(5)
  for i in pos:
    robot.Controller.moveJoint(i[0],i[1])
    delay(5)






```
## Output
### 1. Generic Articulated Robot
![1](https://github.com/Manikandanrag/Movement-of-Robot-Joints/assets/138849491/029f18b4-d4ee-4fee-aa1b-54acb4a73485)


### 2. robot.driveJoints(0,0,0,0,0,0)
![2](https://github.com/Manikandanrag/Movement-of-Robot-Joints/assets/138849491/f1579be6-bac9-4b13-a3a1-d10616d20822)


### 3. Movement of Joint1

![3](https://github.com/Manikandanrag/Movement-of-Robot-Joints/assets/138849491/ced622a5-1d10-49e8-b2d0-257ba5fe8293)


### 4. Movement of Joint2

![4](https://github.com/Manikandanrag/Movement-of-Robot-Joints/assets/138849491/b79ae9f1-9c3c-451a-9241-394f4cec4528)


### 5. Movement of Joint3

![5](https://github.com/Manikandanrag/Movement-of-Robot-Joints/assets/138849491/8feffbf8-dc4a-4164-aafe-3dc72e112b91)

## Result 
Thus the different robots joints are moved with the help of python list.


