# dc-motor-with-h-bridge
dc motors circuit that control a two wheels with a 5v power supply and arduino board 
the simulation of the circuit is done by using tinkercad
* components:
1. power supply
2. arduino uno R3
3. H-bridge motor driver L293D
4. two DC motors
# circuit link:
https://www.tinkercad.com/things/9MUjL2N5tEm-swanky-sango/editel
# circuit figure:
![‏‏لقطة الشاشة (3)](https://user-images.githubusercontent.com/86115930/124303061-a79c8080-db6a-11eb-97df-09521664129f.png)
# circuit code

1. motor define 
- //C++ code
- //MOTOR 1
- #define Ena 10
- #define IN1 9
- #define IN2 8

- //MOTOR 2
- #define Enb 11
- #define IN3 12 
- #define IN4 13

2. pin define 


- pinMode(Ena, OUTPUT);
- pinMode(IN1, OUTPUT);
- pinMode(IN2, OUTPUT);
- pinMode(Enb, OUTPUT);
- pinMode(IN3, OUTPUT);
- pinMode(IN4, OUTPUT);


3. speed control


  - //MOTOR1:
    - digitalWrite(IN1, HIGH);
    - digitalWrite(IN2, LOW);
    - analogWrite(Ena, 120);
  
 - //MOTOR2:
   - digitalWrite(IN3, HIGH);
   - digitalWrite(IN4, LOW);
   - analogWrite(Enb,120);


