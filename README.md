# Software Engineering for Self-Driving Cars Guide :car:
Welcome! This is the ultimate autonomous vehicles guide for all **computer science students**, **software engineers**, or those looking to develop foundational skills for *autonomous vehicle software development*. As an open source project that is continuously updating and improving, we are hoping to provide high-quality, free education for those interested in learning more about autonomous vehicle software development. 

> An autonomous car is a vehicle capable of sensing its environment and operating without human involvement. A human passenger is not required to take control of the vehicle at any time, nor is a human passenger required to be present in the vehicle at all. An autonomous car can go anywhere a traditional car goes and do everything that an experienced human driver does.
[source](https://www.synopsys.com/automotive/what-is-autonomous-car.html)

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
Lorem Ipsum Dolor

### Navigating ###
Lorem Ipsum Dolor

### Sections ###
Lorem Ipsum Dolor

### Tutorials ###
Lorem Ipsum Dolor

### Community ###
Lorem Ipsum Dolor

# Pre-Requisites
For those who are computer science students at a university or a software engineer, it is assumed you have basic data structures and algorthms knowledge. Regardless, this learning guide is for everyone, so below, I have compiled basic knowledge that is important before embarking on this awesome guide. 

- [ ] [Linear Algebra by MIT OpenCourseware](https://ocw.mit.edu/courses/mathematics/18-06-linear-algebra-spring-2010/)
- [ ] [C++](https://www.learncpp.com/) and/or [Python](https://www.coursera.org/specializations/python) programming is expected
- [ ] Data Structures and Algorithms (Cracking the Coding Interview (book) **and/or** [Stanford's Algorithm Course](https://www.coursera.org/specializations/algorithms))
- [ ] [Machine Learning by Andrew Ng](https://www.coursera.org/learn/machine-learning) **and/or** Hands On Machine Learning with Scikit-Learn & Tensor Flow (book) (Recommended, but optional)
- [ ] Basic Git & Linux Command Knowledge (Optional)
- [ ] Basic [Software Development](https://www.ibm.com/topics/software-development) Knowledge (Optional)
- [ ] Familiarize yourself with Embedded Development and Safety Standards (Optional)

# Why Autonomous Vehicles?
Your reasons for using this guide will be unique to you. For me, it was the awe and pure challenge of making a car drive on its own, while also improving my career prospects. A simple reason, which is completely fine. Regardless of your reason for using this guide, here's some motivation and concepts I hope will inspire you even more.

## Motivation :muscle: ##
> "*Whether you think you can, or think you can't, you're right*." - Henry Ford

> "*Self-driving cars are the natural extension of active safety and obviously something we should do*." - Elon Musk

As one of the most debated, challenging, and impactful piece of technology in the automotive industry, developing software for such systems is exciting. Some call self driving car technology the 21st Century Gold Rush.

- **WIRED ARTICLE**: [Self Driving Cars](https://www.wired.com/story/guide-self-driving-cars/)
- **WEBSITE Page**: [The Ethics of Autonomous Cars](https://ethicsofautonomouscars.weebly.com/ethics.html)
- **RESEARCH PAPER**: [A survey of public opinion about self driving vehicles](https://deepblue.lib.umich.edu/handle/2027.42/108384)
- **VIDEO**: [Tesla Self Driving Car Timelapse Drive](https://www.youtube.com/watch?v=tlThdr3O5Qo)


## Our Future :zap: ##
Throughout this guide, it is my goal to provide relevant concepts in psychology and philosophy, as artificial intelligence, AVs, and computer science intersect. One podcast/video I will recommend you watch that I think sheds some light on the future of artificial intelligence and self driving cars is Lex Fridman's interview with Elon Musk.

[The Artificial Intelligence Podcast: Lex Fridman and Elon Musk](https://www.youtube.com/watch?v=dEv99vxKjVI) :robot:

Some key take-aways and quotes from the podcast (thought I highly recommend you listen to it):

1. Lorem Ipsum Dolor 
2. Lorem Ipsum Dolor 
3. Lorem Ipsum Dolor

Though a seemingly bold claim, autonomous vehicles *will* be the future of mobility and transportation. **You can contribute to this future**, which is awesome.

Not only that, but they reduce urban travel time and have a strong environmental impact :sunflower:

## Safety is Critical :vertical_traffic_light: ##
Self-driving cars are safety critical. **_A safety critical system_** can be defined as something that:
>  comprises everything (hardware, software, and human aspects) needed to perform one or more safety functions, in which failure would cause a significant increase in the safety risk for the people or environment involved.

It is easy to acknowledge that autonomous vehicles need to be safe, but as a developer or someone working on self-driving systems, this is  incredibly important to keep in mind. Working with safety critical systems differs greatly from working on a web system. A bug in a web app may prevent users from registering for an account, but a bug in a safety critical system, like a self-driving car, _may result in human fatality unfortunately_. 
<a href="url"><img src="https://user-images.githubusercontent.com/44756122/86859632-139bf400-c091-11ea-917a-1a7d98f841fb.png" align="center" height="300" width="500" ></a>

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

#### Example of a Safety Critical System for Self-Driving Cars ####
* [Advanced Driver Assistance Systems (ADAS)](https://en.wikipedia.org/wiki/Advanced_driver-assistance_systems)
<a href="url"><img src="https://user-images.githubusercontent.com/44756122/86860654-3fb87480-c093-11ea-8931-c280979f38a8.jpg" height="300" width="500" ></a>

Examples of ADAS include [adaptive cruise control](https://www.youtube.com/watch?v=GInSPWZRFRM) and [pedestrian crash prevention](https://www.iihs.org/news/detail/performance-of-pedestrian-crash-prevention-varies-among-midsize-cars). Companies are putting a lot of investment in ADAS, as these systems will be a major component of self-driving cars.

**The gist? Always remember that safety is critical.** If you are interested in learning more about software engineering processes for safety critical systems, I highly recommend you take a look at Phil Koopman's page (linked in the [Resources](https://github.com/tabaddor/av-swe-guide#resources) section).

## High Impact Work :arrow_up_small: ##
Software engineers working on self driving cars will:
* Tackle the hardest challenge of our generation
* Work with cutting edge technology that will impact the lives and safety of people everywhere
* Collaborate with the generation's brightest minds in other engineering fields (electrical, mechanical, systems, etc)

Pumped yet? :muscle:

# Table of Contents
- [ ] [Introduction](https://github.com/tabaddor/av-swe-guide#1-introduction)
- [ ] [Software and Hardware](https://github.com/tabaddor/av-swe-guide#2-software-and-hardware)
- [ ] [Developing for Safety](https://github.com/tabaddor/av-swe-guide#3-developing-for-safety)
- [ ] [Deep Learning for Self-Driving Cars](https://github.com/tabaddor/av-swe-guide#4-deep-learning-for-self-driving-cars)
- [ ] [State Estimation and Localization](https://github.com/tabaddor/av-swe-guide#5-state-estimation-and-localization)
- [ ] [Perception](https://github.com/tabaddor/av-swe-guide#6-perception)
- [ ] [Motion Planning](https://github.com/tabaddor/av-swe-guide#7-motion-planning)
- [ ] [Testing](https://github.com/tabaddor/av-swe-guide#8-testing)

## 1. Introduction ##

## 2. Software and Hardware ##

## 3. Developing for Safety ##

## 4. Deep Learning for Self-Driving Cars ##

## 5. State Estimation and Localization ##

## 6. Perception ##

## 7. Motion Planning ##

## 8. Testing ##


# Resources
- [Carla- Open Source Simulator for AVs](https://carla.org/)
- [ROS- Robot Operating System](https://www.ros.org/)
- [*Embedded Software Development for Safety Critical Systems* by Chris Hobbs](https://www.amazon.com/Embedded-Software-Development-Safety-Critical-Systems/dp/1498726704). (this is not an affiliate link)
- [Software Model Checking with SLAM (report)](https://www.cis.upenn.edu/~alur/CIS673/Spring20/slam11.pdf)
- [Phil Koopman](https://www.youtube.com/channel/UC7QA0wx1m_aLyctDusU4X7g)
- [Deep Learning with Lex Fridman](https://www.youtube.com/watch?v=0VH1Lim8gL8&list=PLrAXtmErZgOeiKm4sgNOknGvNjby9efdf&index=1)


# AV Companies :briefcase:
A list of companies working on autonomous vehicle technologies. The purpose of this section is to include any relevant information about the companies and any open internship and full-time positions. Don't see your company or a position? Submit an issue or pull request!
### Waymo
### Cruise (GM)
### Ford
### Zoox
### Tesla
### Baidu
### Aptiv
### Bosch
### Rivian
### HARMAN International
### May Mobility
### nuro

# What can you do now?
