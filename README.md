# PID-Motor-Control
PID Motor Control System is a system designed to regulate the speed or position of a motor by continuously adjusting the motor's input based on the error between the desired output and the actual output. It will give the user/computer the ability to control the speed and direction of the motor.Basically, it is a basic model of a servo motor.

The hardware platform that we use is the NXP Freedom Development Board (FRDM-KL25Z). The KL25Z is a Cortex-M0+ microcontroller for embedded applications.

Motor Interfacing

The DC motor is connected to the microcontroller board. The motor's power supply and ground connections are then properly connected.We have connected the L298 motor driver for driving the motor if it requires higher current than what the microcontroller can provide.

Sensor Integration

For the sensor, we are using the Optical Rotary Encoder. It provides the feedback on the motor's position or speed.The sensor output is connected to the appropriate input pins of the microcontroller.

PID Algorithm Implementation 

The PID algorithm code is written in C programming language for the FRDM-KL25Z microcontroller board. The code include calculations for the proportional, integral, and derivative terms based on the sensor feedback and desired setpoint. By adjusting the PID gains (Kp, Ki, and Kd), the control system can be fine-tuned to achieve the desired response.

Motor Control by using PWM 

By using the PWM output pins of FRDM-KL25Z, we can generate the control signals for the motor. The PWM signals will adjust the motor's duty cycle to control its speed. 

Feedback Mechanism

By comparing the feedback signals from the sensor with the desired setpoint, we can calculate the error. Feed the error to the code to compute the control output. After getting the output, adjust the motor control signals accordingly.

Fine Tuning 

By observing the motor's response, we can make adjustments to the control gains (Kp, Ki, and Kd) to achieve the desired performance. 
