# Mine-Exploration-Vehicle
Mine Exploration Vehicle designed and implemented using 8086 microprocessor.

##Problem:

A Mine Exploration Vehicle ( MEV) is to be designed. The vehicle is six wheeled with
an on board robotic arm to pick up samples and on board scientific instruments and
cameras (vehicle fig is shown below).
The primary aim of the vehicle is to explore the terrain, measure atmospheric
conditions in the mine and assess samples of rocks and soil. This can be controlled
remotely from above the ground. All subsystems on the vehicle are controlled by the
remote unit and are in contact with the remote unit through a RF modem.
Vehicular motion and Sample collection Subsystem
Each of the six wheels is to be powered by an individual motor so that the vehicle is
capable of climbing over obstacles not exceeding a certain height. The vehicle can
execute a 360°turn in place. The front and rear wheels are used for steering. An
upright position is to be maintained at all times and hence the suspension of the
vehicle cannot have a tilt > 45 °.The tilt is usually not allowed to exceed 30°during
normal operation.The vehicle should be capable of digging up to small depths.
Digging is to be accomplished by spinning one of the front wheels in place to grind
into the soil. The same mechanism that is used for tilting the vehicle upwards is also
used for tilting the vehicle downwards. The vehicle is designed to remain motionless
while the digging wheel is spinning.DC motors are used for rotating the wheels and
stepper motors are used for steering. The two front wheels are locked together by the
same steering mechanism; the same is done in case of the rear wheels.A Robotic arm
is used for sample collection. The robotic arm is capable of movement both in the
horizontal plane and in the vertical plane.Communication of vehicle with surface takes
place through RF modem (CC2420).
Design the necessary hardware and software for implementing the above-mentioned
task.

##ASSUMPTIONS

The following assumptions have been made in designing :

1.The clock frequency is assumed to be given as 2MHz.

2.Due to the non availability of RF modem(CC2420) in proteus,wired transmission
via the keypad on the vehicle has been used to drive the Mine Exploration
Vehicle(MEV).

3.Gyroscope is used to measure the tilt angle which needs to be less than 45°
according to the problem.Since the gyroscope is not available in the proteus library, it
is simulated via a potentiometer.The analog output of gyroscope is simulated using
potentiometer.

##DESIGN SPECIFICATIONS

Mine Exploration Vehicle is a six wheeled rover with a robotic arm designed to pick
up samples and examine using on board scientific instruments and cameras.
The following are the design solution to the given problem:
* Each of the 6 wheels are powered by DC motors.
* 2 Stepper motors are used for the steering system. Stepper motor can be at-tached to
the shaft connecting the two front wheels with the help of the rack and pinion steering
mechanism, thus requiring one stepper motor each for the front wheels and rear
wheels. This also locks the front wheels and the rear wheels as mentioned in the
problem statement.
* This steering system enables the vehicle to climb over obstacles upto a certain height.
An tilt of the vehicle is not allowed to exceed 45 degrees. This is en-sured using a
gyroscope. As soon as the gyroscope records a tilt of 45 degrees of greater, the motor
functions are stopped.
* The digging of the test surface can also be done by moving only the front
wheel. The vehicle is motionless during the digging process.
* The sample of the soil can be examined using the robotic arm. The robotic has 2
DOF in the vertical and the horizontal plane.
* The communication with the vehicle takes place through a RF modem which is
used by the person on the surface operating the vehicle.
* 360 degrees spin in place is done by rotating the left wheels forward and right
wheels back-ward. This is using the differential drive system.
