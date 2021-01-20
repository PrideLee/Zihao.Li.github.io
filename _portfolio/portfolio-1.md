---
title: "Wind-Pendulum System"
# excerpt: "Wind-Pendulum system demo<br/><img src='/images/500x300.png'>"
excerpt: "<video id="video" controls="" preload="none" poster="http://media.w3.org/2010/05/sintel/poster.png">
      <source id="mp4" src="http://media.w3.org/2010/05/sintel/trailer.mp4" type="video/mp4">
      <p>Your user agent does not support the HTML5 Video element.</p>
</video>"
collection: portfolio
---

A wind-pendulum system was designed to controlling four blades' rotate speed to realize specific motion of wind-pendulum, such as line, round, Lissajous figure, cardioid, etc. The hardware includes STM32F103 SCM, swing rod, Cardan joint, laser pointer, keyboard, blades, propeller, MPU6050 Motion Tracking devices, and DC power supply. MPU6050 was used to measure the pendulum angle, then calculate the blades' position by the trigonometric formula. PID control algorithm generates the duty cycle of PWM to control wind pendulum's motion based on the deviation of the real position and expected position.



