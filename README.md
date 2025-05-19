# drone-simulation


>**note:** simulation of drone using full state feedback on MATLAB
>just making this so I do it in the future. This is the initial stage of a bigger project

## Project aim

This project is desgined to keep my control engineering skills up over the summer in preperation for **Advanced Topics in Control of Electromechanical Systems** covered in my upcoming masters.
Through prerequisite study, various methods for this project were explored. Many projects work with real hardware and specifc control problems. However, this project aims to act as a basis for a physical drone/quadcopter design and thus no hardware exists.
This approach will then be to design a system for a "generic" drone design and accomodate variables picked at somewhat random for later tweaking with real hardware.

## Project design:

Initially a model for a quadcopter/drone will be developed in MATLAB designed with basic nessasary components:

- Accelerometer/s
- Gyroscope/s
- Pressure/Barometer
- Ultrasound (optional)
- GPS (likely no need for simulation as it has no relevence to the control due to a resolution of 10m)

  
A flight control system will be developed to control to specifc reference values, in real world implementation these values will be changed with remote control. The flight control system
will be desinged to control the drone roll, pitch, yaw and thrust/altitude.

This project will notably implement control systems thorugh techniques such as:
- PID control
- Kalman state estimation
- Complementary filters
- Low pass filters for noise reduction

Ultimately the system will log movement data in order to plot and visulise the movement of the drone.
