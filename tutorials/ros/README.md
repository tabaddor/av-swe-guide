# ROS Tutorial

What is Robot Operating System (ROS)?

## Environment Setup- Docker ##
- Windows 10 64-bit: Pro, Enterprise, or Education
    - [Docker Desktop on Windows](https://docs.docker.com/docker-for-windows/install/)
- Other Windows Versions
    - [Docker Toolbox on Windows](https://docs.docker.com/toolbox/toolbox_install_windows/)

### Windows ###

#### Installing Docker Toolbox
1. Assuming you meet the requirements in *Step 1: Check your version* of the [Install Docker Toolbox on Windows](https://docs.docker.com/toolbox/toolbox_install_windows/#step-1-check-your-version) guide, download the latest **.exe** file from [Toolbox Releases](https://github.com/docker/toolbox/releases).
2. Run the **Docker Toolbox Installer**
    1. Choose an install location (default is fine)
    2. On *Select Components* page
        - If you already have VirtualBox installed, uncheck it on this page
        - If you already have Git for Windows, no need to install it through the Docker Toolbox installer
    3. On the *Select Additional Tasks* page, use the default checked options, then click Install and then Finish
3. Run **VirtualBox as Administrator**
4. Run **Docker Quickstart Terminal as Administrator**
5. After some installation steps, you should be ready to start!

### Ubuntu ###
Follow the instructions on the Docker website for [Docker Engine - Community](https://docs.docker.com/install/linux/docker-ce/ubuntu/).

### Mac ###
Follow the instructions on the Docker website for [Docker Desktop for Mac](https://docs.docker.com/docker-for-mac/).

## ROS Vocabulary ##
*  **Packages**: Packages are the software organization unit of ROS code. Each package can contain libraries, executables, scripts, or other artifacts.
*  **Manifests**: A manifest is a description of a package. It serves to define dependencies between packages and to capture meta information about the package like version, maintainer, license, etc...
*  **Nodes**: A node is an executable that uses ROS to communicate with other nodes.
*  **Messages**: ROS data type used when subscribing or publishing to a topic.
*  **Topics**: Nodes can publish messages to a topic as well as subscribe to a topic to receive messages.

## Tutorial Steps ##
**NOTE:** If you are using **Docker Toolbox + WSL** as mentioned in in the suggested improvement for Windows, you will need to run **Docker Quickstart Terminal** atleast once to create the **default** virtual machine in VirtualBox. Once this has been created, you will need to manually start the VM since we are not using the quickstart terminal which would have taken care of this for you. In WSL, run `docker-machine.exe start default` and then follow the steps below.

1. In your docker terminal, navigate to the local repository folder
    - `cd /PATH/TO/REPO`
2. Create a docker image called **ros-demo**
    - `docker build -t ros-demo .`
3. Run a container using the ros-demo image
    - `docker-compose run --rm ros-demo`
4. Navigate to the tutorial folder inside your running docker container
    - `cd /tutorial`
5. Set source
    - `source /opt/ros/melodic/setup.bash`

Do all the work inside your **tutorial** folder. This is the only folder linked 
to your host computer. Complete the following [ROS tutorials](https://wiki.ros.org/ROS/Tutorials).

1. [Installing and Configuring your ROS Environment](https://wiki.ros.org/ROS/Tutorials/InstallingandConfiguringROSEnvironment)
    - Skip **1. Install ROS** and **2. Managing Your Environment** as these have already been taken care of in the docker container.
    - For **3. Create a ROS Workspace**, follow the instructions for **catkin** as we are using ROS Melodic which is newer than ROS Groovy.
    - As mentioned previously, all your work should be done inside the **tutorial** folder. In **3. Create a ROS Workspace**, create the catkin workspace inside the tutorial folder rather than the home directory.
        - `mkdir -p catkin_ws/src` instead of `mkdir -p ~/catkin_ws/src`
2. [Navigating the ROS Filesystem](https://wiki.ros.org/ROS/Tutorials/NavigatingTheFilesystem)
    - The ROS tutorial files have already been installed through the **Dockerfile**.
3. [Creating a ROS Package](https://wiki.ros.org/ROS/Tutorials/CreatingPackage)
4. [Building a ROS Package](https://wiki.ros.org/ROS/Tutorials/BuildingPackages)
5. [Understanding ROS Nodes](https://wiki.ros.org/ROS/Tutorials/UnderstandingNodes)
    - Run roscore in the background so you don't need a new terminal window or use tmux as mentioned in **Suggested Improvement (Optional): Docker Toolbox + WSL = tmux**.
        - `roscore &`
    - To run turtlesim, you will need to enable **GUIs for Docker**. See GUIs in Docker section above.
6. [Understanding ROS Topics](https://wiki.ros.org/ROS/Tutorials/UnderstandingTopics)
7. [Understanding ROS Services and Parameters](https://wiki.ros.org/ROS/Tutorials/UnderstandingServicesParams)
8. [Using rqt_console and roslaunch](https://wiki.ros.org/ROS/Tutorials/UsingRqtconsoleRoslaunch)
9.  [Using rosed to edit files in ROS](https://wiki.ros.org/ROS/Tutorials/UsingRosEd)
10. [Creating a ROS msg and srv](https://wiki.ros.org/ROS/Tutorials/CreatingMsgAndSrv)
11. [Writing a Simple Publisher and Subscriber (C++)](https://wiki.ros.org/ROS/Tutorials/WritingPublisherSubscriber%28c%2B%2B%29)

## ROS Commands Wiki ##
- rospack = ros + pack(age) : provides information related to ROS package or stack
- roscd = ros + cd : **c**hanges **d**irectory to a ROS package or stack
- rosls = ros + ls : **l**ist**s** files in a ROS package
- roscp = ros + cp : **c**o**p**ies files from/to a ROS package
- rosmsg = ros + msg : provides information related to ROS message definitions
- rossrv = ros + srv : provides information related to ROS service definitions
- catkin_make : makes (compiles) a ROS package
  - rosmake = ros + make : makes (compiles) a ROS package (if you're not using a catkin workspace)

This tutorial was inspired and based on Michigan Autonomous Aerial Vehicles's ROS Tutorial. For more information, or if at any time you are unclear of how to proceed with this tutorial, please refer to this [repository](https://github.com/MAAV-Software/ros-tutorial).
