# Electronic circuit consits of 6 servo motors 
## parts used in tinkercad
![image](https://github.com/hussein-ak/Electronic-circuit-using-6-servo-motors/assets/173874366/97e1134b-9b93-4773-a673-d8bddf236a79)
## Procedure
### step1 : Assemble hardware components
An Arduino Uno R3, breadboard, six servo motors, and a 6V power supply (four 1.5V AA batteries) have been installed and connected.
### step2 : Arrange servo motors
The six servo motors have been precisely aligned side by side, ensuring optimal positioning for clear and efficient connections in the circuit.
### step 3 : Power setup and servo connections
The 4 AA batteries (6V total) are wired to the breadboard's power rails. Then, each of the 6 servo motors is connected to these rails:

Battery positive → Breadboard (+) rail → Servo positive pins
Battery negative → Breadboard (-) rail → Servo negative pins
This powers all servos uniformly from the central supply.
### step 4 : Connect servo signals and add measurements
Wire each servo's signal pin to Arduino Uno R3 PWM pins (3, 5, 6, 9, 10, 11). 

Additional setup:
• Voltmeter across Servo3 for voltage reading
• Ammeter in series with Servo3 for current measurement

These instruments allow monitoring of Servo3's electrical parameters.
### step5: Programming the Arduino
Code:
#include <Servo.h>

Servo servo1;
Servo servo2;
Servo servo3;
Servo servo4;
Servo servo5;
Servo servo6;

void setup() {
  servo1.attach(3);
  servo2.attach(5);
  servo3.attach(6);
  servo4.attach(9);
  servo5.attach(10);
  servo6.attach(11);
}

void loop() {
  //move each servo to 0 degrees,
  servo1.write(0);
  servo2.write(0);
  servo3.write(0);
  servo4.write(0);
  servo5.write(0);
  servo6.write(0);
  delay(1000);
	//  move to 180 degrees
  servo1.write(180);
  servo2.write(180);
  servo3.write(180);
  //  move to 90 degrees
  servo4.write(90);
  servo5.write(90);
  servo6.write(90);
  delay(1000);
}

## Circuit illustration
### when its off
![image](https://github.com/hussein-ak/Electronic-circuit-using-6-servo-motors/assets/173874366/d5a2dc35-f24b-4860-8ad7-db12abe46783)

### when its on
![image](https://github.com/hussein-ak/Electronic-circuit-using-6-servo-motors/assets/173874366/78e81e0a-20c9-4592-afc9-d2254136eea4)

## link to tinkercad
https://www.tinkercad.com/things/ePAeEJeUNig-glorious-hango/editel?sharecode=skF0Xlj8bkJ6RDD27mgeDeN5VXdc8WnRCOzmTnclFw0

