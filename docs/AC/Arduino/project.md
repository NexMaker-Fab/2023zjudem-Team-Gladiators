<h1 style="font-size:1.7vw"><span style="color:black">A. Project 1</span></h1>
<br>
<h1 style="font-size:1.5vw"><span style="color:black">Project Title: The Smart Proximity Lighting System</span></h1>

 Components needed:

- 1 Arduino Uno
- 1 Breadboard
- 2 LED
- 1 Ultrasonic Distance Sensor

<b>Description:</b>
<br><br>The Smart Proximity Lighting System utilizes a switch-controlled ultrasonic distance sensor to create an intelligent lighting solution. <br>When integrated into home or office environments, the system dynamically adjusts lighting based on the presence or absence of individuals within a specified range. <br>The ultrasonic sensor detects proximity, triggering the switch to seamlessly control the lighting system. <br>This project not only enhances energy efficiency by ensuring lights are only active when needed but also offers a convenient and automated lighting experience. <br>The technology finds applications in home automation, security systems, and various settings where adaptive and energy-conscious lighting is desired. 
<br><div><br><video width=100% height=56.25% controls><source src="image/arp.mp4" type="video/mp4">
</video></div>

   
        int switchState=0;
        long readUltrasonicDistance(int triggerPin, int echoPin) 
        {
        pinMode(triggerPin, OUTPUT);  // Clear the trigger
        digitalWrite(triggerPin, LOW);
        delayMicroseconds(2);
        // Sets the trigger pin to HIGH state for 10 microseconds
        digitalWrite(triggerPin, HIGH);
        delayMicroseconds(10);
        digitalWrite(triggerPin, LOW);
        pinMode(echoPin, INPUT);
        // Reads the echo pin, and returns the sound wave travel time in microseconds
        return pulseIn(echoPin, HIGH);
        }

        void setup()
        {
        pinMode(9, OUTPUT);
        pinMode(10, OUTPUT);
        pinMode(7, INPUT);
        Serial.begin(9600);
        }

        void loop()
        {
        switchState = digitalRead(7);
            if(switchState == 1)
        {
            Serial.println(switchState);
        if (0.01723 * readUltrasonicDistance(4, 3) < 20) {
            digitalWrite(9, HIGH);
            digitalWrite(10, LOW);
        } else {
            digitalWrite(9, LOW);
            digitalWrite(10, HIGH);
        }
        delay(10);
        }
        if(switchState == 0){
            Serial.println(switchState);
        if (0.01723 * readUltrasonicDistance(4, 3) < 20) {
            digitalWrite(9, LOW);
            digitalWrite(10, HIGH);
        } else {
            digitalWrite(9, HIGH);
            digitalWrite(10, LOW);
        }
        delay(10); // Delay a little bit to improve simulation performance
        }
        }

<b>switchState:</b> 
<br><br> An integer variable used to store the state of a switch connected to pin 7.
<br> 
<b>Function Definition:</b>

<b>readUltrasonicDistance(int triggerPin, int echoPin):</b> 
<br>A function that calculates the distance measured by an ultrasonic sensor. It takes two parameters: triggerPin for the trigger pin of the sensor and echoPin for the echo pin of the sensor. It returns the sound wave travel time in microseconds.
Setup Function:

<b>setup():</b> This function runs once when the Arduino board is powered on or reset. It performs the following tasks:
Sets pin 9 and pin 10 as outputs to control external devices.
Sets pin 7 as an input to read the state of a switch.
Initializes the serial communication for debugging purposes.
Loop Function:

    <b>loop():</b>

<br>This function runs repeatedly after the setup() function. It performs the following tasks:
<br>Reads the state of the switch connected to pin 7 and stores it in the switchState variable.
<br>Checks the value of switchState to determine the behavior of the output pins.
<br>If switchState is equal to 1:
<br>Prints the value of switchState to the serial monitor.
<br>Calls the readUltrasonicDistance() function with trigger pin 4 and echo pin 3 as arguments to measure the distance.
<br>Checks if the calculated distance is less than 20 centimeters.
<br>If the distance is less than 20 centimeters, it sets pin 9 to HIGH and pin 10 to LOW.
<br>If the distance is greater than or equal to 20 centimeters, it sets pin 9 to LOW and pin 10 to HIGH.
<br>Adds a delay of 10 milliseconds.
<br>If switchState is equal to 0:
<br>Prints the value of switchState to the serial monitor.
<br>Performs the same distance measurement and control logic as above, but with the opposite output pin states.
<br>Adds a delay of 10 milliseconds.
<br>The code continuously reads the state of a switch and uses an ultrasonic distance sensor to determine the distance of an object.
<br>Depending on the switch state, it controls the output pins (pin 9 and pin 10) to drive external devices based on the measured distance.
<br>The code also outputs the switch state to the serial monitor for debugging purposes.
<br>
<br><b> When Switch is off.</b></div>
<br>
<br><video width=100% height=56.25% controls><source src="image/p2.mp4" type="video/mp4">
</video>
<br>
<br><b> When Switch is on.</b></div>
<br>
<br><video width=100% height=56.25% controls><source src="image/p1.mp4" type="video/mp4"></video>
<br>

<br>
<h1 style="font-size:1.7vw"><span style="color:black">B. Project 2</span></h1>
<br>
<h1 style="font-size:1.5vw"><span style="color:black">Project Title: Fan Control System</span></h1>
<br>
   Components needed:

- 1 Arduino Uno
- 1 Breadboard
- 2 LED
- 4 Resistor 
- 1 DC motor
- 1 LCD screen (16x2)
- 1 Potentiometer (10k ohms)
-  Jumper wires
<br><br><b>Description:</b>
<br><br>The Fan Control System is designed to optimize comfort and energy efficiency by dynamically adjusting fan speeds based on environmental conditions. <br>Utilizing temperature, the system intelligently regulates the fan's operation, ensuring optimal air circulation and cooling. <br>Users can set preferences or allow the system to autonomously respond to changes in the ambient environment. <br>This project is applicable for home automation, offices, and industrial settings, providing a smart and energy-conscious solution for maintaining a comfortable and well-ventilated environment.

<b>How to connect the components in the circuit:</b>

<b>Arduino Connections:</b>
<br><br>The temperature sensor is connected to analog pin A0.
<br>The motor is connected to digital pin 13.
<br>The red LED is connected to digital pin 12.
<br>The green LED is connected to digital pin 11.
<br>The LCD is connected to digital pins 2, 3, 4, 5, 6, and 7.
Once we have completed these connections, we have the components connected according to the code.

<br><b>Here is the result on the tinkercad.</b>
<br><br><video width=100% height=56.25% controls><source src="image/ddd.mp4" type="video/mp4"></video>

    // Libraries included

    #include <LiquidCrystal.h>

    // Declare constants
    const int LM35 = A0;
    const int motor = 13;
    const int LedRed = 12;
    const int LedGreen = 11;

    // initialize the library with the numbers of the interface pins
    LiquidCrystal lcd(2, 3, 4, 5, 6, 7);

    void setup() {
    Serial.begin(9600);
    lcd.begin(16, 2);
    lcd.print("Welcome, Gladiators!");
    pinMode(motor, OUTPUT);
    pinMode(LedRed, OUTPUT);
    pinMode(LedGreen, OUTPUT);
    delay(2000);
    lcd.clear();
    lcd.print("Temp= ");
    lcd.setCursor(0,1);
    lcd.print("Fan= ");
    }

    void loop() {
    int value = analogRead(LM35);
    float Temperature = value * 500.0 / 1023.0;
    lcd.setCursor(6,0);
    lcd.print(Temperature); 
    lcd.setCursor(5,1);
    
    if (Temperature > 50){
        digitalWrite(motor, HIGH);
        digitalWrite(LedRed, HIGH);
        digitalWrite(LedGreen, LOW);
        lcd.print("ON ");
    }
    else {
        digitalWrite(motor, LOW);
        digitalWrite(LedRed, LOW);
        digitalWrite(LedGreen, HIGH);
        lcd.print("OFF");
    }
    
    delay(1000);
    }

<b>Code description</b>

<b>Libraries:</b>
<br>The code includes the necessary library, "LiquidCrystal.h," which allows the Arduino to communicate with and control the LCD display.

<b>Constants:</b> 
<br>Several constants are declared to assign specific pin numbers for the components:

temperature sensor: The analog pin (A0) connected to the temperature sensor.
DC motor: The digital pin (13) connected to the DC motor.
LedRed: The digital pin (12) connected to the red LED.
LedGreen: The digital pin (11) connected to the green LED.

<b>Setup:</b>
<br><br>In the setup() function, the code performs the following tasks:
<br>Initializes the serial communication for debugging purposes.
<br>Initializes the LCD display with the specified number of columns (16) and rows (2).
<br>Prints "Welcome, Gladiators!" on the LCD display at first.
<br>Sets the pin modes for the motor and LEDs as outputs.
<br>Adds a 2-second delay before continuing.
<br>Clears the LCD display.
<br>Prints "Temp= " on the first row and "Fan= " on the second row of the LCD display.

<b>Loop:</b>
<br><br>main functionality of the project is implemented in the loop() function, which continuously repeats the following steps:

<b>Temperature Sensing Section:</b>
<br><br>Reads the analog value from the temperature sensor using analogRead().
<br>Converts the analog value to temperature in degrees Celsius by scaling it using a specific formula.
<br>Updates the LCD display with the temperature reading at the specified positions.

<b>Motor Control Section:</b>
<br><br>Checks if the temperature is greater than 50 degrees Celsius.
<br>If the temperature is above 50, it turns on the motor by setting the motor pin to HIGH and the red LED pin to HIGH. 
<br>The green LED pin is set to LOW.
<br>If the temperature is 50 degrees or below, it turns off the motor by setting the motor pin to LOW and the red LED pin to LOW. The green LED pin is set to HIGH.
<br>Updates the LCD display with the corresponding status ("ON" or "OFF") at the specified position.

<b>Delay:</b>
<br><br>Delays the execution for 1 second before repeating the loop.
<br><br><b>In summary:</b> 
<br><br>This project reads the temperature from the Temperature sensor, displays it on the LCD as shown in the animation, and controls a motor fan and LEDs based on the temperature reading. If the temperature exceeds 50 degrees Celsius, the motor fan and red LED are turned on, indicating a cooling operation. If the temperature is 50 degrees or below, the motor fan and red LED are turned off, and the green LED is turned on, indicating a normal operating condition.
<br>
<br>
<b> Here is the result:</b>
<br>
<br><div class="loader"><img src="image/mlc.jpg" alt="#" width=100% height=56.25%/></div>
<br>

<h1 style="font-size:1.7vw"><span style="color:black">C. Open Source Project</span></h1>
<br>
<h1 style="font-size:1.5vw"><span style="color:black">Project Title: Voice-Controlled Light Switch</span></h1>

[Source](https://www.instructables.com/search/?q=voice%20controlled%20light%20switch&projects=all)

This project is related to our final project.

<b>Description:</b>

Voice-controlled light switch system that allowd users to control the lighting in their home using voice commands. The project involved integrating a voice recognition module with a microcontroller to control the switching of lights.

<b>Components:</b>

Arduino Microcontroller board 
Amazon Alexa Voice recognition module 
Relay module
Light bulbs or LED strips
Power supply
Jumper wires
Functionality:

    <b>Setup:</b>

 the voice recognition module has been connected to the microcontroller board as per the module's instructions, the relay module to the microcontroller board, the light bulbs or LED strips to the relay module, Power the microcontroller board and other components.

<b>Voice Recognition:</b>

The voice recognition module has been trained to recognize specific voice commands for controlling the lights, such as "Turn on/off the lights" or "Dim the lights, Programed the microcontroller to listen for the recognized voice commands from the voice recognition module.

<b>Light Control:</b>

When a voice command is recognized, the microcontroller triggers the corresponding action.
If the voice command is to turn on the lights, the microcontroller activates the relay module, which switches on the connected light bulbs or LED strips.
If the voice command is to turn off the lights, the microcontroller deactivates the relay module, which switches off the lights.
Additional functionality such as dimming the lights or controlling individual lights in different rooms can be implemented based on the specific requirements.

<b>Feedback:</b>

The microcontroller could send a response through a speaker or display a message on an LCD screen confirming the action taken.
With this project, users havev been able to control the lighting in their home by simply speaking voice commands, offering convenience and a hands-free experience.

<b>Advantages of the Voice-Controlled Light Switch project:</b>

<b>Convenience:</b> 

The project offers a hands-free and convenient way to control the lighting in your home. Users can simply use voice commands to turn on/off the lights, eliminating the need for physical switches or remote controls.

<b>Accessibility:</b>

Voice control provides accessibility benefits, particularly for individuals with mobility issues or disabilities, who may find it challenging to reach and operate physical light switches.

<b>Flexibility:</b> 

The project can be customized to control multiple lights or even different types of lights, such as dimming or adjusting the brightness levels. This flexibility allows users to create different lighting scenarios or moods with ease.

<b>Integration with Home Automation Systems:</b> 

This project can serve as a foundation for integrating with larger home automation systems. The voice-controlled light switch can be integrated with other smart devices, such as thermostats, security systems, or voice assistants, to create a comprehensive smart home ecosystem.

<b>Disadvantages of the Voice-Controlled Light Switch project:</b>

<b>Voice Recognition Accuracy:</b>

The accuracy of voice recognition systems can vary based on the specific module or voice assistant used. In some cases, the system may misinterpret or fail to recognize voice commands accurately, leading to incorrect light control.

<b>Dependency on Voice Recognition Module:</b>

The project relies on the proper functioning of the voice recognition module. If the module malfunctions or encounters issues, it may affect the overall performance of the voice-controlled light switch.

<b>Network Dependency:</b>

If the voice recognition module or microcontroller relies on cloud-based voice assistants, such as Amazon Alexa or Google Assistant, a stable internet connection is required for the voice commands to be processed. Network outages or connectivity issues can temporarily disrupt the functionality of the system.

<b>Learning Curve:</b>

Setting up and programming the voice-controlled light switch requires some technical knowledge and familiarity with microcontrollers, voice recognition modules, and programming. Users who are new to these technologies may face a learning curve during the setup and troubleshooting process.



