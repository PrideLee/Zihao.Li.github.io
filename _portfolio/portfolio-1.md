---
title: "Wind-Pendulum System"
excerpt: "Wind-Pendulum System Demo<br/><img src='/images/wind_pendulum.jpg'>"
# excerpt: "Wind-Pendulum system demo<br/><video src='http://media.w3.org/2010/05/sintel/trailer.mp4'>"
collection: portfolio
---

## Abstract

A wind-pendulum system was designed to controlling four blades' rotate speed to realize specific motion of wind-pendulum, such as line, round, Lissajous figure, cardioid, etc. The hardware includes STM32F103 SCM, swing rod, Cardan joint, laser pointer, keyboard, blades, propeller, MPU6050 Motion Tracking devices, and DC power supply. MPU6050 was used to measure the pendulum angle, then calculate the blades' position by the trigonometric formula. PID control algorithm generates the duty cycle of PWM to control wind pendulum's motion based on the deviation of the real position and expected position.

**This problem is from [National Undergraduate Electronic Design Contest - 2015](https://www.nuedc-training.com.cn/index/download/uploadbook/id/64).**

## Demo

[![Wind Pendulum Control System](https://res.cloudinary.com/marcomontalbano/image/upload/v1587315555/video_to_markdown/images/youtube--2qqYywttue4-c05b58ac6eb4c4700831b2b3070cd403.jpg)](https://share.plvideo.cn/front/video/view?vid=a491168bfeeb10853cde2697bcc803f6_a "Wind Pendulum Control System")

You can click [here](https://github.com/PrideLee/Wind-Pendulum) to review the whole project. 


