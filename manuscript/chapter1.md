-# Hardware

# Platform Overview

![](images/rover_small.jpg)

The base platform for the rover is a Parallax robotics shield for the
Arduino, which comes with an aluminium chassis. The shield is mated
with an Arduino Mega 2560, which uses the ATmega2560. The shield has the
standard stacking headers, but also comes with a breadboard and sockets
for up to four servos.

The drivetrain that ships with the shield uses a pair of continuous
rotation servos; the left servo is connected to pin 12 (PB6), while
the right is connected to pin 11 (PB5). The pin selections were chosen
from those available for the servo headers populated on the board;
PB7 is avoided due to the fact that it tends to be pulsed on startup,
which led to a connected servo "twitching" on powerup.

There are currently two sensors on board, both used for distance
measurement. The XL MaxSonar EZ4 ultrasonic ranging sensor is connected
to analog pin 2 (PC2), and the Sharp short-range infrared distance sensor
is connected to analog pin 3 (PC3). Both sensors are mounted on a front
"mast," which can be rotated via a servo connected to pin 10 (PB4).

There are a pair of high-brightness blue LEDs that are used as a visual
beacon that helps in finding the robot. The left beacon is connected to
pin 8 (PH4), and the right beacon is connected to pin 7 (PH5).

In the future, a GPS unit, 4800-baud 434 MHz serial radio, and 9DOF IMU
will be used, but these are not yet connected.

## Pin mapping

