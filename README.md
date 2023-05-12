# Assignment 3 - Jetbot
## Task: Line Following & Object Detection

The aim of the project is to deploy the programmes on the JetBot robot to enable it to perform patrol and object detection tasks. There are two versions of the programmes: the Python version and the ROS version. 
+ The [Python version programme](https://github.com/alstondu/jetbot-ass3/tree/main/Jetbotpy)  is designed to run in Python 3.6 environment. 
+ The [ROS version programme](https://github.com/alstondu/jetbot-ass3/tree/main/jetbot) is implemented as a series of ROS nodes that can be executed individually using `rosrun` or run simultaneously by running a launch file using `roslaunch`.

## Execution Commands
<details open>
<summary>Python Scripts</summary>

The [Line Following + TOF programme](https://github.com/alstondu/jetbot-ass3/tree/main/Jetbotpy/jetbot) to accomplish tasks of line following and obstcale detection.

```commandline
cd ~
cd Jetbotpy/jetbot/
python3.6 LineFollower+TOF.py
```

The [object detection programme](https://github.com/alstondu/jetbot-ass3/tree/main/Jetbotpy/yolov5) to accomplish task of object recognition.

```commandline
cd ~
cd Jetbotpy/yolov5/
python3.6 detect.py
```

</details>


<details open>
<summary>ROS Nodes</summary>

The ROS node initialization.

```commandline
roscore
```

The [Robot_Movement.py](https://github.com/alstondu/jetbot-ass3/blob/main/jetbot/scripts/jetbot/Robot_Movement.py) programme defines a ROS node that subscribles to topics from publishers and controls the movement of the Jetbot.

```commandline
rosrun jetbot Robot_Movement.py
```

The [LF_Publisher.py](https://github.com/alstondu/jetbot-ass3/blob/main/jetbot/scripts/jetbot/LF_Publisher.py) programme defines a ROS node that publishes the line following commands.

```commandline
rosrun jetbot LF_Publisher.py
```

The [TOF_Publisher.py](https://github.com/alstondu/jetbot-ass3/blob/main/jetbot/scripts/jetbot/TOF_Publisher.py) programme defines a ROS node that publishes the TOF commands.

```commandline
rosrun jetbot TOF_Publisher.py
```

The [OR_Publisher.py](https://github.com/alstondu/jetbot-ass3/blob/main/jetbot/scripts/yolov5/OR_Publisher.py) programme defines a ROS node that publishes the Object-Detection commands.

```commandline
rosrun jetbot OR_Publisher.py
```

</details>


<details open>
<summary>ROS Launch File</summary>

ROS launch command execution.

```commandline
roslaunch jetbot jetbot.launch
```

</details>


## Contribution
|Name|Line Following|Obstcale Detection|Object Recognition|ROS Implementation|Code integration|GitHub Repo Maintenance|Attendance|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|Alhuwayji, Abdullah Ahmed A|<span style="color:red">&#10008;</span>|<span style="color:red">&#10008;</span>|<span style="color:red">&#10008;</span>|<span style="color:red">&#10008;</span>|<span style="color:red">&#10008;</span>|<span style="color:red">&#10008;</span>|<span style="color:red">&#10008;</span>|
|Du, Yuang|<span style="color:green">&#10004;</span>|<span style="color:green">&#10004;</span>|<span style="color:red">&#10008;</span>|<span style="color:green">&#10004;</span>|<span style="color:green">&#10004;</span>|<span style="color:green">&#10004;</span>|<span style="color:green">&#10004;</span>|
|Luo, Yanbin|<span style="color:red">&#10008;</span>|<span style="color:red">&#10008;</span>|<span style="color:red">&#10008;</span>|<span style="color:red">&#10008;</span>|<span style="color:red">&#10008;</span>|<span style="color:red">&#10008;</span>|<span style="color:green">&#10004;</span>|
|Stoian, Geanina Nicoleta|<span style="color:green">&#10004;</span>|<span style="color:green">&#10004;</span>|<span style="color:red">&#10008;</span>|<span style="color:red">&#10008;</span>|<span style="color:green">&#10004;</span>|<span style="color:red">&#10008;</span>|<span style="color:green">&#10004;</span>|
|Ye, Zehao|<span style="color:red">&#10008;</span>|<span style="color:red">&#10008;</span>|<span style="color:green">&#10004;</span>|<span style="color:red">&#10008;</span>|<span style="color:green">&#10004;</span>|<span style="color:green">&#10004;</span>|<span style="color:green">&#10004;</span>|

