---
layout: archive
title: "ZIHAO LI-M.S. of University of Chineses Academy of Science"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}


## Education

* **M.S. in Aircraft Design** [Center for Space Utilization (CSU), CAS](http://www.csu.cas.cn/), [The University of Chinese Academic of Science (UCAS)](http://www.ucas.ac.cn/), Sep.2018-Present
* **B.S. in Aircraft Manufacturing Engineering** [College of Mechatronics Engineering](http://jdgc.nuc.edu.cn/#tips), [The North University of Chinal](http://www.nuc.edu.cn/)

## Academic Experience

* **Technology and Engineering Center for Space Utilization (CSU), CAS**, Aug.2017<br />
Reliability & Product Assurance Center, visiting student
  * Scanning Acoustic Microscope (SAM) ultrasonic imaging analysis of aerospace plastic packaging component.
  * Accelerated performance degradation testing and failure mode research for SSD.

* **Xian Jiaotong University - School of Aerospace Engineering**, Aug.2017<br />
Excellent College Students Summer School, visiting student
  * Academic Report: Pollution Dispersion and Water Quality Prediction of Yangtze River.

* **Nationl Space Science Center (NSSC), CAS**, Aug.2017<br />
"One Space, One Dream" Excellent College Students Summer School, visiting student
  * Academic Report: Design and Optimal Control on the No. 3 Chang'e Landing Trajectory.

Internship Experience
======
* **[Aviation Industry Corporation of China (AVIC) - Xian Aircraft industry (Group) Company, LTD](http://www.avic.com/)**, Sep.2017<br />
Graduation Practice, Aircraft Design Intern
  * Assembly process design and optimization of aircraft landing gear.
  * Organize and summarize technical documentation of aircraft design and manufacture.

* **[Guoke Saisi Beijing Tech.co, Ltd.](https://www.cissdata.com/)**, Dec.2017-Aug.2018<br />
Algorithm Engineer in Data Department
  * Electronic components' alternative algorithm research.
  * Bill of Material (BOM) optimization and recommendation.
  * Components classification algorithm research.

## Publications & Patents

[1] **Li Zihao.**  Electronic component data management system and method based on blockchain. China Patent Application [CN109450638A](http://pss-system.cnipa.gov.cn/sipopublicsearch/patentsearch/showViewList-jumpToView.shtml), March 08, 2019.

[2] **Li Zihao.**  Alternative selection system and alternative selection method for electronic components. China Patent Application [CN109284420A](http://pss-system.cnipa.gov.cn/sipopublicsearch/patentsearch/showViewList-jumpToView.shtml), January 29, 2019.

[3] **Li Zihao.**  Form recognition method, recognition system and computer device. China Patent Application [CN109086714A](http://pss-system.cnipa.gov.cn/sipopublicsearch/patentsearch/showViewList-jumpToView.shtml), Dec 25, 2018.

## Projects and Compotetition Experience

* [**Sentiment Analysis**](https://github.com/PrideLee/sentiment-analysis), Project of Deep Learning, Jun.2019
  * Constructing Transformer, text-CNN, and BiGRU+Attention models to analyze the sentiment of movie reviews.
  * Experiments show that CNN turned out to be less efficient on time sequence problems than RNN. While RNN generally takes much more time to train as it does not suit for parallel computation. Transformer proposes a novel approach to deal with NLP tasks. It turns out to have good results and much smoother than RNN.

* [**Repair strategy and Invulnerability Research of Complex Networks**](https://github.com/PrideLee/The-Repair-strategy-and-Invulenrability-Research-of-Complex-Networks), MCM Competition, May.2019
  * The model can provide alternative nodes geographical location information and connection methods when nodes are damaged seriously. Experiments show that the repair strategy can minimize the length of the communication path and ensure network connectivity effectively.
  * First, we calculate the geographical distance between each note based on the Great-circle formula and designing the shortest path connection scheme by the Prim algorithm. In addition, we apply grid search and genetic algorithm (GA) to optimize the path length and providing the alternative nodes numbers, geographical location information as well as connection method when the specified node's failure.
  * Furthermore, relying on the aforementioned research, we add the edges among key nodes, which were determined by the minimum connected dominating the set, to improve the connectivity of the network. Then, with the different number of failure nodes, we simulate the change of path length and connectivity of network with the different number of backup nodes and edges. Finally, considering the path length and network connectivity, we construct an optimal communication network.

* [**Object Detection and Classification**](https://github.com/PrideLee/Object-Detection-and-Classfication), Project of PRML, Nov.2018
  * Constructing YOLO-v3 and FPN networks to realize object detection and recognition.
  * Limited by computing resources, I finetuning the network. Experiments show that on classification tasks, compared with YOLO, FPN has a tiny improvement in accuracy, especially for small objects. While YOLO has a faster speed of training and detection.

* [**Neural Machine Translation (Attention & Transformer)**](https://github.com/PrideLee/Attention-Transformer), Project of NLP, Nov.2018
  * Using the Attention and the Transformer model to realize en2ch machine translation.
  * Considering the performance of the machine, we only select 6834 ch-en pairs (6800s testing samples and 34s testing samples) to analysis the convergence of models and do not comprise the Blue score.
  * Comparing with Attention, Transformer converged after about 30 epochs, and the training process is smoother. In the experiment, the training time of the Transformer is lesser, and the Attention loss is smaller than the Transformer, while in actual situation the result is contrary.

* [**Personalized Matching Model of Packages for Telecom Users**](https://github.com/PrideLee/CCFDF-Personalized-Matching-Model-of-Packages-for-Telecom-Users), CCF-BDCI Competition, Oct.2018
  * Aimed at different users, how to recommend personalized telecommunication packages is a multi-class problem essentially.
  * We extract users' demographic features, behavior features, and preferences through the feature project. In addition, we training random forest (RF), XGBoost and deep network to classify.
  * Experiments show XGBoost has higher F1 values while RF has a shorter training time.
  
* [**Image Recognition Application for Ultrasonic Images of Plastic Packaging IC**](https://github.com/PrideLee/Image-Recognition-Application-for-Ultrasonic-Images-of-Plastic-Packaging-IC), Undergraduate thesis, Aug.2018
  * Aerospace plastic packaging components are in high demand as reliability, and scanning acoustic microscopy screening test is an effective way to ensure the reliability in the space environment. I apply image processing and machine learning technology to segment and recognize the failure ultrasonic image of plastic components.
  * Because of the cost-sensitive and unbalance problem of the data, I provided cost-sensitive learning, which calculated the integrated adjustment ratio to balance the sample distribution. Based on the YOLO network to classified the components, then according to failure standards, I employ image processing technology to extract features. Besides I also train and compare different classifiers' accuracy.
  * Finally, relying on the above research, I developed a failure recognition tool of plastic part acoustic scanning image to reduce the operating pressure of technicians.
  
* [**Plate-and-Ball Control System**](https://github.com/PrideLee/Plate-and-Ball-control-system), Electronic Design Contest, Aug.2017
  * Based on steering engine control technology, PID (proportional plus integral plus derivative) control algorithm, images processing technology and single-chip development, we designed and achieved a plate-and-ball control system, which collects the ball position and motion information by a camera, as actuator, linkage mechanism  driven by steering engine controls tilts the plate, then controlling the ball to finish specific motion.
  * The hardware includes camera support, STM32F4, steering engine, OV7670 camera, linkage, keyboard, and DC power supply.
  * The system adopts a single loop PID control strategy, the camera collects the real position information then calculating the position deviation. Based on it, we utilize the PID algorithm to get the duty cycle of PWM, through this signal to drive the steering engine. Therefore, we can control the tilt of the plate to plan the motion track of the ball.  
  
* [**Wind-Pendulum**](https://github.com/PrideLee/Wind-Pendulum), Electronic Design Contest, Jul.2017
  * We design a wind-pendulum, through controlling four blades' rotate speed to realize specific motion of wind-pendulum, such as line, circle, Lissajous figure, cardioid, etc.
  * The hardware include STM32F103, swing rod, cardan joint, laser pointer, keyboard, BLDC, propeller, MPU6050, and DC power supply.
  * Using MPU6050 measures the pendulum angle, then we calculate the position of BLDC by the trigonometric formula. Based on the deviation of the position, the PID algorithm outputs the duty cycle of PWM to control the motion of wind-pendulum.
  
* [**"Internent+" Based Subsidy Scheme  Optimization of Ridesharing**](https://github.com/PrideLee/The-subsidy-scheme-of-DiDi), MCM Competition, Sep.2016
  * With internet technology developed rapidly, many ridesharing apps were developed nowadays. Hence, optimizing subsidy and dispatch schemes of taxies will be helpful to ease the difficulty of hailing taxies.
  * Taking Shenzhen as a sample, we crawled taxies driving information from ridesharing websites. Besides, we defined supply and demand ratio of taxies, taxi ownership (ten thousand people), and the empty-loaded rate to investigate the matching degree between taxi sources and public requirements in the different time and geographical locations.
  * Based on the psychological model and fuzzy mathematics, we build a membership function to reflect the relation between subsides and driver, passenger satisfaction. Furthermore, we also consider companies' costs to adjust and optimize the subsidy aimed at rush hour and remote areas. Our subsidy scheme can balance the benefit of drivers, passengers, and software companies well.
  

## Selected Honors & Awards

### Competition Awards

* Oct.2017, **2nd Award**, National Undergraduate Electronic Design Contest
* Aug.2017, **Excellence Award**, The 11th National College Student Mechanics Competition
* Jan.2017, **onorable Mention**, Mathematical Contest in Modeling (Intrenational)
* Nov.2016, **2nd Award**, Mathematical Contest in Modeling (China)
* Nov.2015, **First Prize**, The 7th National College Student Mathematical Competition

### Scholarship

* Jun.2018, **First Class**, Outstanding Graduate Scholarship
* Jan.2017, **First Class**, Hubei Chamber of Commerce Encouragement Scholarship
* Oct.2016, **First Class**, Comprehensive Quality Scholarship
* Oct.2015, **First Class**, National College Student Mathmatical Competition Scholarship

## Skills

* Programming: Python, C/C++, Matlab
* Data Processing & Database: SPSS Clementine, MySQL, Excel
* Computer-Aided Design and Modeling: AutoCAD, ProE, SolidWorks
* SCM Development and Circuit Design: STM32F4, STC89C52RC, Altium Designer
* Others: LINGO, Git, LaTeX, Adobe Photoshope, Adobe Captivate

## Languages

* English: TOEFL, Preparing
* Chinese: Native or Bilingual Proficiency

<!--
Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
-->

<!-- Talks
======
  <ul>{% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>
-->


**CV can be downloaded <a href=""><u>here</u></a>**

