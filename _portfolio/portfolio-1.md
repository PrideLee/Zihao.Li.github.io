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

<video id="video" controls="" preload="none" poster="https://share.plvideo.cn/front/video/view?vid=a491168bfeeb10853cde2697bcc803f6_a">
      <source id="mp4" src="https://share.plvideo.cn/front/video/view?vid=a491168bfeeb10853cde2697bcc803f6_a" type="video/mp4">
      <p>Your user agent does not support the HTML5 Video element.</p>
</video>

You can click [here](https://github.com/PrideLee/Wind-Pendulum) to review the whole project. 


