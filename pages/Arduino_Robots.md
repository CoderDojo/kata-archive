This page is about using low-cost Arduino Robots to teach computer
science.

Here is a list of some of the general concepts we teach with our Robots:

1.  Compiling code
2.  Deployment
3.  Debugging
4.  Variables
5.  Variable Scope
6.  Functions and Subroutines
7.  Naming Functions
8.  Passing Parameters to Functions

Our goal is to create low-cost (under $25 USD) robot kits that students
can build and program with Arduino and Scratch. We use the mblock IDE to
generate Arduino code from Scratch.

We have moved the Robot Assembly instructions to the Instructables web
site site
here;

<http://www.instructables.com/id/Collision-Avoidance-Robot-for-Teaching-Programming/>

The code is now available on github here:

<https://github.com/dmccreary/coderdojo-robots>

We are working on an on-line book here:

<https://dmccreary.gitbooks.io/coderdojo-robots/content/>
<http://coderdojo-robots.readthedocs.io/en/latest/>

The Arduino labs can be extended to teach the basics of robotics.

In Minnesota we start with 20 labs using the SparkFun Inventors Kit. We
are now extending these with a $25 basic robot kit based on a simple
three wheel two motor platform.

## Lab 1 - The H-Bridge and a Motor Control Chip

Goal: Move a motor in two directions - forward and backwards Our next
step is to introduce the basic concept of an H-Bridge to change motor
direction. A good example of this is to use the L293D to teach the
concept of moving a motor forward and backward.

### Lab Resources

  - [Wikipedia page on H-Bridges](http://en.wikipedia.org/wiki/H_bridge)
  - [Arduion Motor Control H-Bridge L293D
    Lab](http://www.instructables.com/id/Control-your-motors-with-L293D-and-Arduino/)
  - [Adafruit descrition of the
    L293D](http://www.adafruit.com/product/807)
  - [$12.00 Robot Kit on
    E-Bay](http://www.ebay.com/itm/Motor-New-Smart-Robot-Car-Chassis-Kit-Speed-Encoder-Battery-Box-For-Arduino-/361060892190)

## Lab 2 - Programming a Robot to Move

Code to move a robot forward, backward, turn right and turn left.

## Lab 3 - Adding an LED Strip

The LED strip provides feedback about what data the robot is seeing. We
are using a short 12 segment strip of WS2812B (aka NeoPixel) to display
sensor data.

## Lab 4 - Adding a Ping Sensor

We then add an Arduino Nano (with USB) and a breadboard.

Next we add a ping sensor.

Here is some basic example code:

  - [Robot Code on
    GitHub](https://github.com/dmccreary/coderdojo-robots/src/v1/robot_ping_led/robot_ping_led/robot_ping_led.ino)

## Lab 5 - Basic Collision Avoidance Robot

In this lab we connect the motor control, sensor and LED strip together
to build a robot that moves up to and obstacle and turns right.

  - [Sample Code on
    GitHub](https://github.com/dmccreary/coderdojo-robots/blob/35cb43944d59b04b205491d001a90c2dd4c065c3/src/v1/robot_ping_led/robot_ping_led/robot_ping_led.ino)

## Additional Resources

[Twin Cities Arduino GitHub](https://github.com/CoderDojoTC/arduino)

[Dan's
blog](http://datadictionary.blogspot.com/2014/11/robot-kits-for-coderdojo-labs.html)
on robot kits.
