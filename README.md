	Course: Microprocessor System (Lab)
	
	Project name: Voice Controlled Car Using Tiva-C TM4C123GH6PM Launchpad 
	
	Description: The purpose of this project was to develop a robot which can operate on voice commands. To transmit voice commands from our 
	phone to the microcontroller (Tiva-C TM4C123GH6PM Launchpad), Bluetooth Module HC-05 was used which used UART communication protocol for 
	data transmission. UART Module 4 of the microcontroller was used for this purpose. To power the tyres of this robot car, 4 motors were 
	being controlled using L298N Dual H-Bridge Motor Driver. Their speed was controlled by PWM signal generated by the microcontroller. 2 Timer 
	modules were being used for this purpose --> TIMER2 & TIMER3. To ensure safety of the microcontroller from the back emf generated from motor
	incase it is disconnected suddenly, optocouplers were used which made sure that the microcontroller was isolated from the motors. Another 
	feature added to the robot was the distance measurement which made it stop when it got closer (less than 5cm) to any obstacle. For this purpose,
	we used Ultrasonic Sensor HC-SR04. The data was digitally collected so there was no need for analog to digital conversion. To sum up, this 
	robot can work on some specified commands which are stated as follows.
	1. Forward   --> Moves the car at 50% duty cycle in forward direction
	2. Backward	 --> Moves the car at 50% duty cycle in reverse direction
	3. Go Fast   --> Moves the car at 75% duty cycle in forward direction
	4. Go Faster --> Moves the car at 100% duty cycle in forward direction
	5. Slow Down --> Moves the car at 25% duty cycle in forward direction
	6. Left      --> Changes the direction to left and moves it in forward direction
	7. Right     --> Changes the direction to right and moves it in forward direction
	8. Stop      --> Stops the movement
	It is to be noted that the car doesn't work continously. For every command given to this robot, it will perform it and then stops after
	a maximum of 3 seconds (in case of changing direction). 
	
	Power Requirement: HC-05 & HC-SR04 are connected in paralled with a 9V battery. They can be connected with any source providing a 
	minimum of 5V. However the microcontroller & the motor driver L298N are powered with two 9V battery in series, providing 18V in total.
	For the optocouplers, a 9V battery is providing the VCC & GND to their circuit. 
	
	Team Members: 	Aziz Haider
	
	Use KEIL IDE Software to test your version of code onto the TM4C123GH6PM Launchpad
