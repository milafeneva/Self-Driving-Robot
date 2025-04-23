# Self-Driving-Robot
Creation of an algorithm for controlling the Lego Mindstorm EV3 robot 
https://drive.google.com/drive/folders/1fdkjAe5p5xFWcE1J2BcoAaH4c_GKoAPC

Overview:
This project involves the development of an autonomous robot capable of navigating a predefined path marked by a black line (road) using active opto-sensors. The robot is equipped with additional functionalities, including obstacle detection using an ultrasound sensor and the ability to overtake obstacles, as well as an integrated camera for parking spot detection in a designated parking lot.
Functionalities:
The robot employs a rule-based line-following algorithm to stay centered on the black line. It utilizes data from five active opto-sensors (one centered and two on each side) to make real-time decisions on motor control. If the center sensor detects the line, the robot moves forward. If either side sensor detects a deviation, the robot adjusts its direction accordingly, either turning left or right. The robot utilizes an ultrasound sensor to detect obstacles or other robots in its path. A rule-based classifier determines the appropriate action. If an obstacle is detected, the robot executes an overtaking maneuver by turning left, moving forward, turning right, and returning to the line. As the robot reaches the end of the road, it enters a parking lot equipped with a camera. The camera captures images of the parking lot, and a classifier is employed to identify empty parking spots.

I. Introduction 
Steps
1. Path following with opto sensors 
The robot utilizes a rule-based line-following algorithm with five active opto-sensors to navigate a predefined path marked by a black line. The center sensor guides forward movement, while side sensors detect deviations, prompting adjustments in direction.
2. Obsticle detaction using ultrasound sensor
The robot employs an ultrasound sensor to detect obstacles or other robots in its path. A rule-based classifier determines the appropriate action in response to detected obstacles.
3. Overtaking part 
 If an obstacle is detected, the robot executes an overtaking maneuver by turning left, moving forward, turning right, and returning to the line.
4. Parking spot detection with integrated camera 
As the robot reaches the end of the road, it enters a parking lot equipped with a camera. The camera captures images of the parking lot, and a classifier is employed to identify empty parking spots.
In the realm of robotics and artificial intelligence, our project stands at the forefront of innovation, presenting a cutting-edge solution to autonomous navigation challenges. The central idea revolves around the development and design of an autonomous robot capable of seamlessly traversing a predefined path marked by a black line, akin to a road, utilizing sophisticated active opto-sensors. Beyond mere navigation, this intelligent robot is equipped with additional functionalities that elevate its capabilities, including obstacle detection through ultrasound sensors, overtaking maneuvers, and even parking spot identification using an integrated camera.
To bring this concept to life, our team has meticulously crafted a rule-based line-following algorithm that serves as the brain behind the robot's precise movements. Employing data from five strategically positioned active opto-sensors, the robot makes real-time decisions on motor control. The primary sensor, centered on the robot, guides its forward motion, while the two sensors on each side ensure it stays on course. Should a deviation be detected, the robot adeptly adjusts its direction, executing turns with unparalleled accuracy.
Beyond the realm of the black line, the robot incorporates an ultrasound sensor, adding a layer of obstacle detection sophistication to its repertoire. A rule-based classifier interprets the sensor data, enabling the robot to make informed decisions when faced with impediments. In the face of obstacles, the robot executes a series of calculated moves, including turning left, advancing, turning right, and seamlessly returning to the designated path.
As the robot nears the end of its journey, it enters a designated parking lot, where an integrated camera takes center stage. This camera captures images of the parking lot, and a sophisticated classifier is employed to identify vacant parking spots. It is this amalgamation of advanced sensors, rule-based algorithms, and integrated functionalities that positions our autonomous robot project on the vanguard of autonomous navigation technology, showcasing the remarkable possibilities within the intersection of robotics and artificial intelligence.
Our project pioneers innovation in robotics and artificial intelligence through the development of an autonomous robot. Designed for precise line-following using active opto-sensors, the robot seamlessly navigates a predefined path, demonstrating unparalleled accuracy in turns and deviations.
Beyond basic navigation, the robot incorporates ultrasound sensors for obstacle detection and executes calculated maneuvers in response. Additionally, an integrated camera identifies vacant parking spots as the robot approaches the end of its journey.
Powered by a rule-based line-following algorithm, this project showcases the integration of advanced sensors, rule-based algorithms, and diverse functionalities, positioning it at the forefront of autonomous navigation technology.
II. Related Work
What inspired us? 
Our first inspiration was an article about a car parking monitoring system using wireless sensor networks.
Here is the link to the article: https://publications.waset.org/17079/a-car-parking-monitoring-system-using-wireless-sensor-networks

Our second inspiration is a real-time obstacle avoidance method for an autonomous vehicle. This new obstacle avoidance method for autonomous vehicles, called obstacle-dependent Gaussian potential field, was designed and implemented for detecting obstacles. 
This article inspired us to get more in-depth with our first idea, and we came up with an idea for our robot to not just be able to self-park but be able to avoid and overtake obstacles as well. 
Obstacle avoidance is one of the essential technologies in local path planning and one of the critical technologies that guarantees human and vehicle safety. For decades, many research studies have been performed on this theme and many methods have been developed, a few of which have been implemented in real systems. In order to avoid collision with obstacles, a robot needs not only to detect obstacles but also to recalculate the detouring path and to steer itself toward a safe and efficient path in real time.
https://www.hindawi.com/journals/jat/2018/5041401/
This really interesting article was an improved version of our idea for over-taking obsticles. Our vehicle uses sensors in order to recognize the obsticle in front of it. 
The following picture is a representation of a host vehicle overtaking an obsticle vehicle using a combined action of attraction and repulsion.
Last article; 
https://www.frontiersin.org/articles/10.3389/fnbot.2023.1269447/full

III. Concept of operation 
The steps we will use in order to get to the final results (use diagrams and scenarios) block diagram 
Explanation of formulas and avoiding an obstacle: https://journals.sagepub.com/doi/full/10.1177/17298806221115984 

IV. System requirements 
Activity diagram 
 
