# Software Engineering for Self-Driving Cars Guide :car:
Welcome to the ultimate autonomous vehicles guide for all **computer science students**, **software engineers**, or those looking to develop foundational skills for *autonomous vehicle software development*. As an open source project that is continuously updating and improving, we are hoping to provide high-quality, free education for those interested in learning more about autonomous vehicle software development. 

> An autonomous car is a vehicle capable of sensing its environment and operating without human involvement. A human passenger is not required to take control of the vehicle at any time, nor is a human passenger required to be present in the vehicle at all. An autonomous car can go anywhere a traditional car goes and do everything that an experienced human driver does.
[source](https://www.synopsys.com/automotive/what-is-autonomous-car.html)

# Table of Contents
## Introduction ##
- [ ] [How to Contribute/Guidelines](https://github.com/tabaddor/av-swe-guide#how-to-contribute)
- [ ] [Getting Started](https://github.com/tabaddor/av-swe-guide#getting-started-w-the-guide-tada)
- [ ] [Prerequisite Resources](https://github.com/tabaddor/av-swe-guide#pre-requisites-and-resources)
- [ ] [Autonomous Vehicles Motivation](https://github.com/tabaddor/av-swe-guide#why-autonomous-vehicles)
## Guide ##
- [ ] [Introduction](https://github.com/tabaddor/av-swe-guide#1-introduction)
- [ ] [Software and Hardware](https://github.com/tabaddor/av-swe-guide#2-software-and-hardware)
- [ ] [Developing for Safety](https://github.com/tabaddor/av-swe-guide#3-developing-for-safety-traffic_light)
- [ ] [Deep Learning for Self-Driving Cars](https://github.com/tabaddor/av-swe-guide#4-deep-learning-for-self-driving-cars)
- [ ] [State Estimation and Localization](https://github.com/tabaddor/av-swe-guide#5-state-estimation-and-localization)
- [ ] [Perception](https://github.com/tabaddor/av-swe-guide#6-perception)
- [ ] [Motion Planning](https://github.com/tabaddor/av-swe-guide#7-motion-planning)
- [ ] [Testing](https://github.com/tabaddor/av-swe-guide#8-testing)
## Resources/FAQ ##
- [ ] [Resources](https://github.com/tabaddor/av-swe-guide#resources-1)
- [ ] [AV Companies](https://github.com/tabaddor/av-swe-guide#av-companies-briefcase)
- [ ] [What can you do now?](https://github.com/tabaddor/av-swe-guide#what-can-you-do-now)
- [ ] [FAQ](https://github.com/tabaddor/av-swe-guide#faq-speech_balloon)

# How to Contribute
:white_check_mark: This is an open source guide, so contributions are very much welcome. To contribute:

Fork this repository and clone the repository
```
git clone https://github.com/YOUR-USERNAME/av-guide
```

Change into the repository's directory
```
cd av-guide/
```

Make the changes on your forked version, and then submit a pull request which will be reviewed shortly after. 

# Contribution Guidelines
View the complete contribution guidelines, [here](contributing.md).

#### Wait! Don't forget to give this project a star! ####
![recording](https://user-images.githubusercontent.com/44756122/84942050-449b9100-b0b0-11ea-9a2c-5736759b25e9.gif)

# Getting Started w/ the Guide :tada:
### Introduction ###
You can use this guide however you like. If you prefer to follow along material by material, go ahead. If you want to skip ahead, come back, skip ahead again, do as you wish. To get started with basic navigation and resources, briefly skim through the below tips.

### Navigating ###
Navigating this project should be fairly straightforward and simple. But, to help you along any struggles along the way, here is how to navigate to some specific things:

#### README Document ####
This [README](https://github.com/tabaddor/av-swe-guide) document is the central documenation for this guide. At the top, is the Table of Contents which you can use as a main directory. 

#### Contributing Document ####
The [contributing document](https://github.com/tabaddor/av-swe-guide/blob/master/contributing.md) provides details regarding contributing guidelines, issues, feature requests, and the repository vision. Before submitting an issue or pull request, please briefly review it.

#### Tutorials ####
**On the GitHub page, the tutorials can be found in the ['tutorials'](https://github.com/tabaddor/av-swe-guide/tree/master/tutorials) folder**

**To work locally, first clone the repository page, and simply cd into the tutorial root directory:**
```
cd av-swe-guide/tutorials/<tutorial-name>
```

#### Resources ####
Other resources outside of the structured roadmap this project compiles include YouTube channels, open source github projects (like Carla simulator). To be specific:
1. [Resources](https://github.com/tabaddor/av-swe-guide#resources) (Links to YouTube channels, research papers, documentation, GitHub projects, and more that are touched upon in the guide)
2. [Full-Time and Internship Opportunties](https://github.com/tabaddor/av-swe-guide#av-companies-briefcase) :briefcase:
3. Self Driving Car Company Developments and Research

### Sections ###
The table of contents of this guide is [here](https://github.com/tabaddor/av-swe-guide#table-of-contents) in this README document. Feel free to jump around from section to section,
or skim through a section's resource. These sections will be continuously updating and improving with new material and resources. 

### Tutorials :book: :robot: ###
The purpose of the tutorials is to provide hands-on learning working with tools and technologies covered in or related to material in the guide contents. For example, though Robot Operating System (ROS) is not explicity covered in a dedicated section, it's a popular middleware used in robotics that's a handy thing to know.

_Have a suggestion for a tutorial not covered? Want to suggest an edit for a current tutorial?_ Submit and issue and pull request!

### Community :speech_balloon: ###
As this community grows, [@tabaddor](https://github.com/tabaddor) will look into creating a community Slack and/or Discord. For the time being, all communication will be exclusively on GitHub.

# Pre-Requisites (and resources)
For those who are computer science students at a university or a software engineer, it is assumed you have basic data structures and algorthms knowledge. Regardless, this learning guide is for everyone, so below, I have compiled basic knowledge that is important before embarking on this awesome guide. 

- [ ] [Linear Algebra by MIT OpenCourseware](https://ocw.mit.edu/courses/mathematics/18-06-linear-algebra-spring-2010/)
- [ ] [C++](https://www.learncpp.com/) and/or [Python](https://www.coursera.org/specializations/python) programming is expected
- [ ] Data Structures and Algorithms (Cracking the Coding Interview (book) **and/or** [Stanford's Algorithm Course](https://www.coursera.org/specializations/algorithms))
- [ ] [Machine Learning by Andrew Ng](https://www.coursera.org/learn/machine-learning) **and/or** Hands On Machine Learning with Scikit-Learn & Tensor Flow (book) (Recommended, but optional)
- [ ] [Basic Git & Linux Command Knowledge](https://www.linux.com/topic/desktop/introduction-using-git/) (Optional)
- [ ] Basic [Software Development](https://www.ibm.com/topics/software-development) Knowledge (Optional)
- [ ] Familiarize yourself with Embedded Development and Safety Standards (Optional)

# Why Autonomous Vehicles?
Regardless of your reason for using this guide, here's some motivation and concepts I hope will inspire you.

## Motivation :muscle: ##
> "*Whether you think you can, or think you can't, you're right*." - Henry Ford

> "*Self-driving cars are the natural extension of active safety and obviously something we should do*." - Elon Musk

As one of the most debated, challenging, and impactful piece of technology in the automotive industry, developing software for such systems is exciting. Some call self driving car technology the 21st Century Gold Rush.

- **WIRED ARTICLE**: [Self Driving Cars](https://www.wired.com/story/guide-self-driving-cars/)
- **WEBSITE Page**: [The Ethics of Autonomous Cars](https://ethicsofautonomouscars.weebly.com/ethics.html)
- **RESEARCH PAPER**: [A survey of public opinion about self driving vehicles](https://deepblue.lib.umich.edu/handle/2027.42/108384)
- **VIDEO**: [Tesla Self Driving Car Timelapse Drive](https://www.youtube.com/watch?v=tlThdr3O5Qo)


## Our Future :zap: ##
Though a seemingly bold claim, autonomous vehicles *will* be the future of mobility and transportation. **You can contribute to this future**, which is awesome.

Not only that, but they reduce urban travel time and have a strong environmental impact. :sunflower:

## Safety is Critical :vertical_traffic_light: ##
Self-driving cars are safety critical. **_A safety critical system_** can be defined as something that:
>  comprises everything (hardware, software, and human aspects) needed to perform one or more safety functions, in which failure would cause a significant increase in the safety risk for the people or environment involved.

It is easy to acknowledge that autonomous vehicles need to be safe, but as a developer or someone working on self-driving systems, this is  incredibly important to keep in mind. Working with safety critical systems differs greatly from working on a web system. A bug in a web app may prevent users from registering for an account, but a bug in a safety critical system, like a self-driving car, _may result in human fatality unfortunately_. 
<img src="https://user-images.githubusercontent.com/44756122/86859632-139bf400-c091-11ea-917a-1a7d98f841fb.png" align="center" height="650px" width="800px" >

#### IOS 26262 Safety Standard ####
To mitigate risk for developers, teams and companies developing safety critical systems typically have to follow safety standards, such as ISO 26262.
[ISO 26262](https://www.iso.org/standard/43464.html) is one of the more well-known safety standards that you should be aware of regarding autonomous vehicles. 

I recommend briefly skimming through [ISO 26262](https://www.iso.org/standard/43464.html) to get an idea of the standard, but to summarize some key points:
* The goal is to ensure safety throughout the lifecycle of automotive system development
* Code you write as a developer must be in line with the safety standard (companies and teams specify this for you)
* There are specific steps of ISO 26262, and other standards, that are required in each phase of the software development lifecycle

_Standards aid in making sure the code you write as a developer is carefully evaluated, inspected by others, and tested during the development process to mitigate risk_. This is an essential component of software engineering for any safety critical system, as a lot of emphasis is placed on "careful coding."

One way to look at the challenge of developing self-driving cars is that it seems as if there are "infinite" edge cases. This is exciting, yet one of the bigger challenges that self-driving cars face.

**VIDEO**: [The Real Moral Dilemma of Self Driving Cars](https://www.youtube.com/watch?v=WBjY3QGNdAw)
**RESEARCH PAPER**" [Self Driving cars and the urban challenge](https://github.com/tabaddor/av-swe-guide#faq)

#### Example of a Safety Critical System for Self-Driving Cars ####
* [Advanced Driver Assistance Systems (ADAS)](https://en.wikipedia.org/wiki/Advanced_driver-assistance_systems)
<img src="https://user-images.githubusercontent.com/44756122/86860654-3fb87480-c093-11ea-8931-c280979f38a8.jpg" height="650px" width="800px">

Examples of ADAS include [adaptive cruise control](https://www.youtube.com/watch?v=GInSPWZRFRM) and [pedestrian crash prevention](https://www.iihs.org/news/detail/performance-of-pedestrian-crash-prevention-varies-among-midsize-cars). 

**The gist? Always remember that safety is critical.** If you are interested in learning more about software engineering processes for safety critical systems, I highly recommend you take a look at Phil Koopman's page (linked in the [Resources](https://github.com/tabaddor/av-swe-guide#resources) section).

## High Impact Work :arrow_up_small: ##
Software engineers working on self driving cars will:
* Tackle the hardest challenge of our generation
* Work with cutting edge technology that will impact the lives and safety of people everywhere
* Collaborate with the generation's brightest minds in other engineering fields (electrical, mechanical, systems, etc)

Pumped yet? :muscle:

# 1. Introduction #
This introductory section will provide high level overviews about the history of autonomous vehicles, basic autonomous vehicle taxonomy/terminology, and the current state of self-driving cars. This section is not overly technical, but interesting and important nonetheless.

Below is a typical software stack for a self-driving car. It should be pretty self-explanatory, however, **don't get bogged down in the details**, it _will_ all fit together at the end (taken from Hyundai-Aptiv Webinar).

![hyundai-aptiv-webinar-softwarestack](https://user-images.githubusercontent.com/44756122/87368175-efd22580-c54a-11ea-95a1-c39cd482e9e3.PNG)

#### History of Autonomous Vehicles :scroll: ####
- [ ] [A Brief History of Autonomous Vehicle Technology](https://www.wired.com/brandlab/2016/03/a-brief-history-of-autonomous-vehicle-technology/)
- [ ] [The Story of Autonomous Vehicles](https://www.coursera.org/lecture/intro-self-driving-cars/the-story-of-autonomous-vehicles-pEfib)

#### Taxonomy ####
- [ ] [How do self-driving cars work?](https://robohub.org/how-do-self-driving-cars-work/)
- [ ] [Taxonomy of driving](https://www.coursera.org/lecture/intro-self-driving-cars/lesson-1-taxonomy-of-driving-BdNR6)
- [ ] [Driving Decisions and Actions](https://www.coursera.org/lecture/intro-self-driving-cars/lesson-3-driving-decisions-and-actions-vPSnD)

#### Levels of Autonomy :oncoming_automobile: ####
![levelsofautonomy](https://user-images.githubusercontent.com/44756122/87369758-3fb2eb80-c54f-11ea-9fe0-67e8e4c5c813.png)


**Summary**:
- [ ] [Self-Driving Car](https://en.wikipedia.org/wiki/Self-driving_car)
- [ ] [Public Health, Ethics, and Autonomous Vehicles](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5343691/)
- [ ] [The Future of Autonomous Vehicles](https://www.coursera.org/learn/intro-self-driving-cars/lecture/HdaOV/the-future-of-autonomous-vehicles)
- [ ] [State of the Art: Self-Driving Cars w/ MIT's Lex Fridman](https://www.youtube.com/watch?v=sRxaMDDMWQQ&list=PLrAXtmErZgOeY0lkVCIVafdGFOTi45amq)

### Section Terminoloy: ###
- **Sensors:** A device or machine whose purpose is to detect events or changes in its environment and record or respond to the data.
- **Computer Vision (Perception):** A field of artificial intelligence that trains computers to interpret and understand the visual world.
- **Controls:** Manipulation of forces by way of steering, braking, etc. Needed to execute guidance commands to maintain vehicle stability.
- **Planning:** Planning a path, mission, or behavior of the vehicle and predictions of its surrounding.
- **Mobility as a Service (MaaS):** A shift from personally-owned modes of transportation and towards mobility provided as a servie.
- **OTA Software Update:** Distributing new software over an encrypted network. Tesla does this with their vehicle fleets.
- **ADAS:** Advanced Driver Assistance Systems. Electronic systems that help the vehicle driver while driving or during parking.
- **Connected Vehicle:** A car that can communicate with other systems outside of the car. Most cars are connected these days in some shape or form.
- **Datasets:** Collection of data to use in the development and testing of autonomous sytems (example: traffic data, weather data, pedestrian data, etc)
[A complete gloassary of Automated Vehicle Terms](http://www.cts.virginia.edu/wp-content/uploads/2018/03/Glossary-of-CAV-Terms-Ver1.0-03052018-1.pdf)



# 2. Software and Hardware  #
As a software engineer working on self driving car technology, **it is important you have an understanding of not only the software, but the hardware involved**. You don't need to be an expert in computer architecture or circuits, but a general understanding and appreciation of hardware is important. With that said, let's dive into the software and hardware architecture of self-driving cars.

### Sensors and Hardware Architecture :battery: ###
- [ ] [Sensors and Computing Hardware](https://www.coursera.org/lecture/intro-self-driving-cars/lesson-1-sensors-and-computing-hardware-LrLty)
- [ ]  [Three Sensor Types of Autonomous Vehicles](https://www.fierceelectronics.com/components/three-sensor-types-drive-autonomous-vehicles)

**Hardware in the Loop (HiL)**

**_Hardware in the Loop_** is a technique that is used in the development and testing of _real-time embedded systems_. Working as a software or computer engineer at a self-driving car compnay, you may work on the Hardware in the loop team.
- [ ] [What is Hardware in the Loop? (video)](https://www.youtube.com/watch?v=BrmqyVuyegc)
- [ ] [Hardware in the Loop](https://en.wikipedia.org/wiki/Hardware-in-the-loop_simulation)
- [ ] [Hardware in the Loop simulation for autonomous vehicles](https://www.researchgate.net/publication/241157481_Hardware-in-the-loop_simulation_for_autonomous_driving)
- [ ] [HIL Simulator for Developing Automated Driving Algorithms](https://ieeexplore.ieee.org/document/8123155)

Below is an image of the various sensors in Google's self driving car. **Sensors** are devices which mesaure some sort of physical property and records or responds to the data.

<img src="https://user-images.githubusercontent.com/44756122/87368706-6c193880-c54c-11ea-82c3-6b2f1311be8f.png" style="height: 650px; width: 800px;" />

**Sensors** work together to provide the car with visuals of its surroundings to ultimately help detect pedestrians, other cars, etc and feeds the data into learning algorithms that aid with motion planning and path prediction. You'll work with the actual computer vision algorithms that deal with the sensor data and images in the [Perception](https://github.com/tabaddor/av-swe-guide#6-perception) section, but for now, just understand how this piece of hardware ties into the self-driving vehicle as a whole. **_Read [HERE](https://blogs.nvidia.com/blog/2019/04/15/how-does-a-self-driving-car-see/) for more information about how a self-driving car uses sensors to see._**

### Software Architecture ###
_The high level idea_ behind self-driving car software architecture and stacks is separating the main vehicle functionalities into modules (perception, planning, and controls), and allowing them to work together/communciate. 
- [ ] [Software Architecture for Self-Driving Cars](https://www.coursera.org/lecture/intro-self-driving-cars/lesson-1-sensors-and-computing-hardware-LrLty)
- [ ] [IEEE Accelerating Autonomous Vehicles](https://spectrum.ieee.org/transportation/self-driving/accelerating-autonomous-vehicle-technology)
- [ ] [Stanford Autonomouos Vehicle Technical Stack Video (**great summary**)](https://www.youtube.com/watch?v=V8LA0_bb9LI)

![autoware-selfdrivingunit-stack](https://user-images.githubusercontent.com/44756122/87736188-8437c480-c7a5-11ea-801a-a6085fdb654d.png)


### Section Tutorials and Projects: ###
- [ ] [ROS (Robot Operating System) Tutorials](https://github.com/tabaddor/av-swe-guide/tree/master/tutorials/ros)

**Section Terminology:**
- **LiDar vs. Radar:** _LiDar_ is a method for measuring distances by illuminating the target with laser light and measure the reflection with a sensor. _Radar_ uses
radio waves to achieve the same task. [LiDar vs Radar for Applied Autonomy](https://semcon.com/offerings/applied-autonomy/lidar-vs-radar-for-applied-autonomy/)
- **Sensors:** A device or machine whose purpose is to detect events or changes in its environment and record or respond to the data.
- **Hardware in the Loop:** A simulation technique used in the development and testing of real-time embedded systems.
- **Software Stack:** A set of software subsystems and components needded to develop and complete a platform. Most self-driving car software stacks follow the same idea.
- **Computing Hardware:**
- **CPU/GPU**: A central processing unit and a graphical processing unit that work together, sitting atop the compute hardware to carry out instructions and concurrent data.
- **Sensor Fusion:** The ability to bring data from multiple inputs (cameras, LiDar, Radar, etc) to form a single model of the environment around the vehicle.
- **Mapping:** Using sensor data to form "maps" of the environment around the vehicle. 



# 3. Developing for Safety :traffic_light: #
Like stressed earlier in the motivation section, **_SAFETY IS CRITICAL_**. As a software engineer or developer working on autonomous, safety critical systems, it's especially important your code applies to safety standards, is tested rigorously (manually and automatically), and more which will be covered in this section. 

### Safety Assurance for Self-Driving Cars ###
- [ ] [Safety Assurance for Autonomous Vehicles](https://www.coursera.org/learn/intro-self-driving-cars/lecture/gtsMT/lesson-1-safety-assurance-for-self-driving-vehicles)
- [ ] [Safety Frameworks for Driving](https://www.coursera.org/learn/intro-self-driving-cars/lecture/hCttH/lesson-3-safety-frameworks-for-self-driving)
- [ ] [How Many Miles Would it Take to Demonstrate AV Reliability?](https://www.rand.org/pubs/research_reports/RR1478.html)

Unfortunately, _sometimes_ things go wrong. That is the challenege.
* [Uber Crash Preliminary Report](https://www.ntsb.gov/investigations/AccidentReports/Reports/HWY18MH010-prelim.pdf)


### Software Engineering Activites:computer: ###
As a software engineer, _only around 10% to 30% of your time will be spent actually writing new code_. The remaining time will be spent reading, understanding, debugging, testing, and communicating code. That is why, especially for a safety critical system like a self-driving car, you have a solid understanding of software engineering activities. We will focus on the big three that are: Testing, Code Quality and Metrics, and Productivity. 

### Testing ###
Testing is expensive. But it is also crucial for self-driving cars. Testing the vehicle modules as a whole may take place in simulations, but you will still need the basics of software development testing down. 

- [ ] [Software Engineering at Goolge](https://arxiv.org/ftp/arxiv/papers/1702/1702.01715.pdf)
- [ ] [Code Coverage](https://en.wikipedia.org/wiki/Code_coverage)
- [ ] [Software Development Lifecyle in 9 minites](https://www.youtube.com/watch?v=i-QyW8D3ei0)
- [ ] [Autonomous Vehicle Virtual Testing and Validation](https://www.youtube.com/watch?v=hP9rYv6p9aA)

You'll hear the terms [**_validation_** and **_verification_**](https://en.wikipedia.org/wiki/Verification_and_validation), and be aware that though the sound similar, they are widely different terms. **Validation** involves making sure your system meets requirements. **Verification** invovles making sure your software system is correct. Validation and verification can go hand in hand. 

**Static Analysis**- Debugging that is done by examining the code without executing the program
- [ ] [Static Program Analysis](https://en.wikipedia.org/wiki/Static_program_analysis)
- [ ] [A Decade of Software Model Checking with SLAM](https://dijkstra.eecs.umich.edu/kleach/eecs481/readings/slam.pdf)

**Dynamic Analysis**- Testing and evaluation by executing the data in real-time
- [ ] [Dynamic Program Analysis](https://en.wikipedia.org/wiki/Dynamic_program_analysis)


### Code Quality/Metrics ###
What is defined as quality code and how quality code is measured will differ from organization to organization, and maybe even from team to team. Is your goal bug-free code? Is your goal minimal debugging time? Is your goal less lines of code? These are all things managers and teams consider, and important for you as a developer to keep in mind when working on safety critical systems like self-driving cars.
- [ ] [Quality Assurance](https://en.wikipedia.org/wiki/Quality_assurance)
- [ ] [State of Mutation Testing at Google](https://dijkstra.eecs.umich.edu/kleach/eecs481/readings/mutation-google.pdf)
- [ ] [145 Questions for Data Scientist in Software Engineering](https://dijkstra.eecs.umich.edu/kleach/eecs481/readings/datase.pdf)

### Productivity/Teamwork ###
For the most part, you won't be working on a system alone. You'll be on a team, and a lot of times, coding with another developer in what is called _pair programming._ Pair programming involves two developers working on a feature, issue, etc, however, they work on their own parts, and then convene later on to discuss and communicate. 
- [ ] [Cost and Benefits of Pair Programming](https://dijkstra.eecs.umich.edu/kleach/eecs481/readings/pairprogramming.pdf)


### Dr. Phil Koopman- a gold mine of autonomous vehicle safety research and information: ###
His YouTube channel can be found in the [Resources section](https://github.com/tabaddor/av-swe-guide#resources). Here are some noteworthy vehicles I recommend:
- [ ] [Software Maintenance Best Practices](https://www.youtube.com/watch?v=raXfwiOKySo)
- [ ] [10 Risks of Poor Embedded Software Quality](https://www.youtube.com/watch?v=aclkJqBK2HM)
- [ ] [Software Testing Best Practices](https://www.youtube.com/watch?v=GKrp1Ab6doc)
- [ ] [Best Practices for Unit Testing](https://www.youtube.com/watch?v=Qkzjmgn8zto)
- [ ] [Embedded Software Security, Safety, and Quality](https://www.youtube.com/watch?v=elK0GJUm958)

**VIDEO/INTERVIEW**: [Speaking of Psychology: Self-Driving Cars](https://www.apa.org/research/action/speaking-of-psychology/self-driving-cars)


### Section Tutorials and Projects: ###
- [ ] [Testing Tutorial](https://github.com/tabaddor/av-swe-guide/tree/master/tutorials/testing)(_Note: This is the same tutorial listed in the [Testing](https://github.com/tabaddor/av-swe-guide#8-testing) section_)

### Section Terminology: ###
- **Safety:** Condition of being protected, unlikely to cause or be at risk of danger, injury, or death. 
- **Testing:** Activity involved placing your code under rigurous edge cases that allows you to assess the code quality.
- **Metrics:** Measurement that allows you to place objective judgement on pieces of code.
- **Code Maintainability:** Ensuring that code is readable by other developers, low in defects, and low coupling (how related code is).
- **Code Readability:** How easy code is to follow logically by developers other than the original author. 
- **Code Reliability:** Reliable code is secure and handles exceptions for a segment of code accordingly. 
- **Test Suite/Cases:** _A test suite_ is a collection of test cases intended to test a segment or feature of code. _A test case_ is comprised specific units of execution to test the
correctness of a piece of code. 
- **Software Quality:** How well the code conforms to a design and the requirements/specifications. What is defined as "quality code" tends to differ from company to company as most
use different metrics to measure code quality. 
- **Unit Testing:** Testing individual units of the source code at a time. 
- **Integration Testing:** Testing where individual software modules are combined for testing together. 
- **Mutation Testing:** Involves modifying a test case and seeing if that "mutant" passes or fails when run against the source code. 



# 4. Deep Learning for Self-Driving Cars #
The resources in this section will be enough to get started with deep learning. Remind you, it takes _years_ to understand/master the concepts in ML and deep learning.

The high level idea behind Deep Learning is building machine learning algorithms and functions that mimic the human brain in processing data for tasks including object detection, speech recognition, and decision making. If you haven't already, I highly recommend you check out [Stanford's Machine Learning Course](https://www.coursera.org/learn/machine-learning) for free. Also, [**this**](https://github.com/tabaddor/Machine-Learning) has some great resources compiled for machine learning, deep learning, and computer vision.

**Machine Learning and Deep Learning** are such large fields, with a lot of infomration. Don't feel overwhelmed, but try to read as much as you can, and code as much as you can. Here is a [page containing resources for Machine Learning, Deep Learning, and Computer Vision.](https://github.com/tabaddor/Machine-Learning)

### Machine Learning Overview ###
- [ ] [What is Machine Learning?](https://www.coursera.org/learn/machine-learning/lecture/Ujm7v/what-is-machine-learning)
- [ ] [Supervised Learning](https://www.coursera.org/learn/machine-learning/lecture/1VkCb/supervised-learning)
- [ ] [Unsupervised Learning](https://www.coursera.org/learn/machine-learning/lecture/olRZo/unsupervised-learning)
- [ ] [Classification](https://www.coursera.org/learn/machine-learning/lecture/wlPeP/classification)
- [ ] [Stanford CS229 Machine Learning](http://cs229.stanford.edu/)
- [ ] [University of Michigan EECS 445 Machine Learning](https://eecs445-f16.github.io/)
- [ ] [University of Michigan EECS 445 Machine Learning Resources](https://github.com/eecs445-f16/umich-eecs445-f16)

### Neural Networks ###
- [ ] [What is a Neural Network?](https://www.coursera.org/learn/neural-networks-deep-learning/lecture/eAE2G/what-is-a-neural-network)
- [ ] [Non-Linear Hypothesis](https://www.coursera.org/learn/machine-learning/lecture/OAOhO/non-linear-hypotheses)
- [ ] [Neurons and the Brain](https://www.coursera.org/learn/machine-learning/lecture/IPmzw/neurons-and-the-brain)
- [ ] [Neural Network Model Representation](https://www.coursera.org/learn/machine-learning/lecture/ka3jK/model-representation-i)

### [**First Neural Network for Beginners Explained (with code)**](https://towardsdatascience.com/first-neural-network-for-beginners-explained-with-code-4cfd37e06eaf) :brain:

### [**Neural Networks from Scratch**](https://medium.com/towards-artificial-intelligence/building-neural-networks-from-scratch-with-python-code-and-math-in-detail-i-536fae5d7bbf)

A specifc class of Neural Networks you should familiarize yourself with are Convolutional Neural Networks, which are involved in tasks including object detection, image processing, classification, and image segmentation.
### Convolutional Neural Networks ###
- [ ] [An Intuitive Explanation of Convolutional Neural Networks](https://ujjwalkarn.me/2016/08/11/intuitive-explanation-convnets/)
- [ ] [One Layer of a Convolutional Neural Network](https://www.coursera.org/lecture/convolutional-neural-networks/one-layer-of-a-convolutional-network-nsiuW)
- [ ] [Simple CNN Example](https://www.coursera.org/lecture/convolutional-neural-networks/simple-convolutional-network-example-A9lXL)
- [ ] [Why Convolutions?](https://www.coursera.org/lecture/convolutional-neural-networks/why-convolutions-Xv7B5)
- [ ] [Feedforward Neural Networks]()

Choose from **at least one** of the below:
1. ### [MIT's Deep Learning for Self Driving Cars](https://deeplearning.mit.edu/)
2. ### [Convolutional Neural Networks for Visual Recognition](http://cs231n.stanford.edu/)

### Section Tutorials/Projects ###
Will be updated. Expect projects to work with implementing basic machine learning models, neural networks, and computer vision.

### Section Terminology ###
- **Machine Learning:** A subset of artificial intelligence that provides a computer, or system, the ability to improve its performance on a task by learning from experience.
- **Supervised Learning:** A type of machine learning task that is provided labeled training data (both x and y are known).
- **Unsupervised Learning:** A type of machine learning task that is provided unlabeled training data (only y is known).
- **Classification Problems:** A machine learning task that involves discrete valued output ("boy" or "girl"; "dog" or "cat").
- **Regression Problems:** A machine learning task that involves continuous/numerical valued output ("find the expected housing price given this data")
- **Gradient Descent:** An optimization algorithm for finding the local minimum of a differentiable function. When we say machine learning algorithms involve slow altering of a function (hypothesis) to converge to the optimal output, we are referring to this idea of gradient descent.
- **Deep Learning:** A subset of machine learning that bases its methods off of artificial neural networks with representation learning. 
- **Neural Network:** Algorithms based off the biological neural networks, designed to mimic the way the human brain operates. Neural networks are meant to adapt to input and generate the best possible result without needing to redesign the machine learning model/algorithm. 
- **Convolutional Neural Network:** A class of neural networks applied to visual imagery such as object detection.
- **Stochastic Gradient Descent:** A deterministic approximation to gradient descent. Much more effieicnt algortihm that iteratively computes gradient descent as traditionally defined. 

# 5. State Estimation and Localization #
State estimation is the problem of determining the current **state** of a system, such as a vehicle. Localization is the implementation of algorithms for state estimation with an error of less than a small, non-zero value. 

### Least Squares ###
- [ ] [Squared Error Criterion and the Method of Least Squares](https://www.coursera.org/lecture/state-estimation-localization-self-driving-cars/lesson-1-part-1-squared-error-criterion-and-the-method-of-least-squares-zDFtr)
- [ ] [Squared Error Criterion and the Method of Least Squares - Part 2](https://www.coursera.org/lecture/state-estimation-localization-self-driving-cars/lesson-1-part-2-squared-error-criterion-and-the-method-of-least-squares-Ewy9K)
- [ ] [Recursive Least Squares](https://www.coursera.org/learn/state-estimation-localization-self-driving-cars/lecture/0UbTb/lesson-2-recursive-least-squares)
- [ ] [Research on Lane Change Decision for Autonomous Vehicles Based on Multi-Kernels Least Square Policy Iteration](https://ieeexplore.ieee.org/abstract/document/8047653)

### State Estimation and Kalman Filters ###
- [ ] [Introduction to Kalman Filters and Its Applications](https://www.intechopen.com/books/introduction-and-implementations-of-the-kalman-filter/introduction-to-kalman-filter-and-its-applications)
- [ ] [The Kalman Filter](https://www.coursera.org/lecture/state-estimation-localization-self-driving-cars/lesson-1-the-linear-kalman-filter-7DFmY)
- [ ] [The Extended Kalman Filter](https://www.coursera.org/learn/state-estimation-localization-self-driving-cars/lecture/qIyk3/lesson-3-going-nonlinear-the-extended-kalman-filter)
- [ ] [Basic Kalman Filter in C++](https://github.com/hmartiro/kalman-cpp)

### Pose Estimation ###
- [ ] [3D Geometry and References Frames](https://www.coursera.org/learn/state-estimation-localization-self-driving-cars/lecture/ccy3B/lesson-1-3d-geometry-and-reference-frames)
- [ ] [Pose Estimation of a Textured Object](https://docs.opencv.org/master/dc/d2c/tutorial_real_time_pose.html)
- [ ] [TensorFlow C++ Pose Estimation](https://github.com/jenshemprich/tf-cpp-pose-estimation)
- [ ] [Why Sensor Fusion?](https://www.coursera.org/learn/state-estimation-localization-self-driving-cars/lecture/HCP35/why-sensor-fusion)

### LiDar Sensing ###
You may have heard that Elon Musk and Tesla stay away from LiDar for their own reasons, one being that LiDar is expensive. Well, it used to be expensive. LiDar is becoming less expensive and is best suited for self-driving cars.

- [ ] [Light Detection and Ranging Sensors](https://www.coursera.org/learn/state-estimation-localization-self-driving-cars/lecture/3NXgp/lesson-1-light-detection-and-ranging-sensors)
- [ ] [LiDar Sensing Models and Point Clouds](https://www.coursera.org/learn/state-estimation-localization-self-driving-cars/lecture/Huunu/lesson-2-lidar-sensor-models-and-point-clouds)
- [ ] [Pose Estimation from LiDar Data](https://www.coursera.org/learn/state-estimation-localization-self-driving-cars/lecture/XE9kZ/lesson-3-pose-estimation-from-lidar-data)

### Section Tutorials/Projects ###
Will be updated.

### Section Terminology ###
- **State Estimation and Localization:** State estimation involves determining the state of an object, vehicle, or self. Localization is essentially how a vehicle figures out its location, or where it is, whch involves using its on-board cameras and sensors to estimate positions.
- **Least Squares:** Minimize the squared difference between an observed and expected values.
- **Pose Estimation:** Is a subset of computer vision that involves locating and tracking the position of an object or specific parts of an object.
- **Kalman Filter:** A KF provides estimates of some unknown signal overtime given previously determined measurements for that signal, or correlated signals.
- **LiDar Sensing:** Illuminate a target object with a laser light, and then measure the reflection.
- **Sensor Fusion:** Ability to bring together multiple inputs from multiple different sensors to construct one world model and understanding of an environment.
- **Point Clouds:** A set of data points in space that represent a 3D shape or object.

# 6. Perception #
For the purposes of this guide, perception and computer vision are synonymous. Perception deals with training our vehicle to perceive its environment in order to act on what it perceives. How does it perceive its environment? **With sensors**. And how does the vehicle make sense of the sensor data? **With computer vision algorithms.**

### Computer Vision ###
- [ ] [Computer Vision for Autonomous Vehicles **HIGHLY RECOMMENDED**](https://arxiv.org/pdf/1704.05519.pdf)

Today, there are two main ways of performing vision: Classical vision and machine learning. This guide will provide resources for understanding and working with both methods.

##### Classical Vision #####
- [ ] [OpenCV Tutorials for Classical Vision](https://docs.opencv.org/master/d9/df8/tutorial_root.html)

##### Vision with Deep Learning #####
Make sure you have first gone through the Deep Learning section to understand the underlying theory and concepts. 

- [Deep Learning for Computer Vision: University of Michigan All Lectures](https://www.youtube.com/watch?v=dJYGatp4SvA&list=PL5-TkQAfAZFbzxjBHtzdVCWE0Zbhomg7r)

### Sensors and Cameras ###
- [The Camera Sensor](https://www.coursera.org/lecture/visual-perception-self-driving-cars/lesson-1-part-1-the-camera-sensor-ziCGj)

### Camera Calibration ###
- [Camera Calibration](https://www.coursera.org/learn/visual-perception-self-driving-cars/lecture/EEu6i/lesson-2-camera-calibration)
- [Image Filtering](https://www.coursera.org/learn/visual-perception-self-driving-cars/lecture/AMoYz/lesson-4-image-filtering)
- [Image Features and Feature Descriptors](https://www.coursera.org/learn/visual-perception-self-driving-cars/lecture/V7iCJ/lesson-1-introduction-to-image-features-and-feature-detectors)

### Object Detection ###
- [Object Detection Guide](https://www.fritz.ai/object-detection/)
- [Gentle Introduction to Object Detection with Machine Learning](https://machinelearningmastery.com/object-recognition-with-deep-learning/)
- [YOLO Original Paper](https://www.cv-foundation.org/openaccess/content_cvpr_2016/html/Redmon_You_Only_Look_CVPR_2016_paper.html)

### Semantic Segmentation ###

### Section Tutorials/Projects ###

### Section Terminology ###
- **Computer Vision:** How can computers understand a situation based on images? CV is all about extracting and making use of interesting and important features of an image, which is really just made up on pixels which can be represented as vectors/matrices, to ultimately interpret an environment.
- **Sensors:** Devices that perceive the environment and provide information to actuators or algorithms which make sense of the data received via the sensors. For computer vision, sensors include cameras, radars, and LiDar. 
- **Object Detection:** Related to computer vision and image processing that deals with detecting instances of objects in a given frame or image.
- **Image Segmentation:** Identify every pixel that belongs to a specific object in a frame or image.
- **Classical Vision:** Classical techniques for computer vision involve leveraging and extracting features of an image or frame without the use of ML or DL.
- **Convolutional Neural Networks:** A type of Deep Learning algorithm suited for images and computer vision tasks. More info on CNN's [here](http://yann.lecun.com/exdb/publis/pdf/lecun-bengio-95a.pdf).

# 7. Motion Planning #

### The Problem ###
Motion planning, also known as **path planning**, is the the problem of finding a sequence of valid motions, configurations, steps, etc that allow an agent to go from its source location to goal destination. Motional planning has several key applications in robotics and autonomous vehicles, rightfully so. In this section, we will break down some key aspects of this function.

### Planning ###
- [ ] [Robotics: Computational Motion Planning](https://www.coursera.org/learn/robotics-motion-planning)
- [ ] [EECS 367 Autonomous Robotics Course at the University of Michigan Homepage](https://autorob.org/)
- [ ] [Path Planning Algorithms in C++](https://github.com/vss2sn/path_planning)

### Mapping ###
- [ ] [Simultaneous Localization and Mapping (SLAM) Paper: Essential Algorithms](https://people.eecs.berkeley.edu/~pabbeel/cs287-fa09/readings/Durrant-Whyte_Bailey_SLAM-tutorial-I.pdf)
- [ ] [Visual SLAM Resources](https://github.com/tzutalin/awesome-visual-slam)

### Dynamic Objects ###

### Section Tutorials/Projects ###

### Section Terminology ###

# 8. Testing #

### Importance of Testing ###

### Unit Testing ###

### Integration Testing ###

### Static and Dynamic Analysis ###

### Simulation ###

# Bonus: Mathematics for Self-Driving Cars #
Mathematics is fundamental to most engineering concepts, especially those involved in designing and testing the systems of AVs. Here are a few key resources and topics to review if you are interested.

### Linear Algebra ###
- [MIT Open Courseware](https://ocw.mit.edu/courses/mathematics/18-06-linear-algebra-spring-2010/)
- [Khan Academy](https://www.khanacademy.org/math/linear-algebra)

### Statistics ###
- [MIT Open Courseware](https://ocw.mit.edu/courses/mathematics/18-443-statistics-for-applications-spring-2015/)

### Information Theory ###

# The Most Important Thing #
Languages will come and go. Frameworks will come and and go. Tools and technologies will come and go. Understanding the idea, theory, and/or mathematics behind the concepts, rather than memorizing snippets of code, is the most important thing. 


# Resources
- [Carla- Open Source Simulator for AVs](https://carla.org/)
- [ROS- Robot Operating System](https://www.ros.org/)
- [*Embedded Software Development for Safety Critical Systems* by Chris Hobbs](https://www.amazon.com/Embedded-Software-Development-Safety-Critical-Systems/dp/1498726704). (this is not an affiliate link)
- [Phil Koopman](https://www.youtube.com/channel/UC7QA0wx1m_aLyctDusU4X7g)
- [Deep Learning with Lex Fridman](https://www.youtube.com/watch?v=0VH1Lim8gL8&list=PLrAXtmErZgOeiKm4sgNOknGvNjby9efdf&index=1)
- [Beyond the Code - Machines, Algorithms, and Life](https://gobeyondthecode.com)
- [openpilot: Open Source Driver Assistance Software](https://comma.ai/)


# AV Companies :briefcase:
A list of companies working on autonomous vehicle technologies. The purpose of this section is to include any relevant information about the companies and any open internship and full-time positions. Don't see your company or a position? Submit an issue or pull request!
### Waymo ###
[Waymo](https://waymo.com/) is an autonomous driving technology company that is a subsiduary of Alphabet, Inc. 

[**Open Roles**](https://waymo.com/joinus/)

### Cruise
[Cruise](https://www.getcruise.com/) is a self-driving car company owned by General Motors (GM).

[**Open Roles**](https://www.getcruise.com/careers/software)

### Ford
[Ford](https://www.ford.com) Motor Company is an American automaker now building hybrid and electric vehicles, AVs, SUVs, and Crossovers.

[**Open Roles**](http://corporate.ford.com/careers.html?gnav=footer-aboutford)

### Zoox
[Zoox](https://zoox.com/) is an American Autonomous Vehicle company now a subsiduary of Amazon.

[**Open Roles**](https://zoox.com/join/)

### Tesla
[Tesla](https://www.tesla.com/) is an electric car and solar/clean energy company.

[**Open Roles**](https://www.tesla.com/careers)

### Aptiv
[Aptiv](https://www.aptiv.com/) is an autoparts company shaping the future of mobility through green, connected ADAS and AV technology.

[**Open Roles**](https://www.aptiv.com/careers/students-and-graduates)

### Rivian
[Rivian](https://rivian.com/) is an electric vehicle manufacturer also working on AV technology.

[**Open Roles**](https://rivian.com/careers)

### HARMAN International
[HARMAN International](https://www.harman.com/) is a Samsung subsiduary focusing on car lifesyle, audio, and connected products, including ADAS.

[**Open Roles**](https://jobs.harman.com/)

# What can you do now?
Some inspirational, yet concrete advice coming your way. Lorem Ipsum Dolor.

# FAQ :speech_balloon:
#### Q: Who can use this guide? ####
A: This guide is mainly geared towards computer science students and software engineers looking to learn more about the self-driving car industry. With that said, 
anyone is welcome to embark on the guide, just make sure you have an understanding of the [pre-requisites](https://github.com/tabaddor/av-swe-guide#pre-requisites-and-resources).

#### Q: How do I get started with this guide and roadmap? ####
A: Get started [here](https://github.com/tabaddor/av-swe-guide#software-engineering-for-self-driving-cars-guide-car)! Have fun learning! Official guide content starts [here](https://github.com/tabaddor/av-swe-guide#1-introduction), but the introductions are important.

#### Q: Can I download this guide? ####
A: You may clone and work with this project on your local machine. In fact, if you want to complete the tutorials, that is recommended. Get started with [this](https://github.com/tabaddor/av-swe-guide/blob/master/contributing.md#how-can-i-contribute) to create your own fork.

#### Q: I have a suggestion, how can I contribute to this guide? ####
A: Contribitions and suggestions are always welcome. First, read through this [contributing document](https://github.com/tabaddor/av-swe-guide/blob/master/contributing.md), then submit an issue and/or pull request.

#### Q: I don't know much about computer science/software, how can I still use this? ####
A: Like stated in a previous question, this guide assumes a certain level of knwoledge of computer science and software engineering concepts. Feel free to learn those, however, in the future, we are looking at developing tutorials that introduce other engineering fields (electrial, mechanical, systems, etc).
