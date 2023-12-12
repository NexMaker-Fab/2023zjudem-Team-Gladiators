<h1 style="font-size:1.7vw"><span style="color:black">A. Project 1</span></h1>
<br>
<h1 style="font-size:1.5vw"><span style="color:black">Project Title: The Smart Proximity Lighting System</span></h1>

<p> Components needed:</p>
<ul>
<li>1 Arduino Uno</li>
<li>1 Breadboard</li>
<li>2 LED</li>
<li>1 Ultrasonic Distance Sensor</li>
</ul>
<p><b>Description:</b>
<br><br>The Smart Proximity Lighting System utilizes a switch-controlled ultrasonic distance sensor to create an intelligent lighting solution. <br>When integrated into home or office environments, the system dynamically adjusts lighting based on the presence or absence of individuals within a specified range. <br>The ultrasonic sensor detects proximity, triggering the switch to seamlessly control the lighting system. <br>This project not only enhances energy efficiency by ensuring lights are only active when needed but also offers a convenient and automated lighting experience. <br>The technology finds applications in home automation, security systems, and various settings where adaptive and energy-conscious lighting is desired. </p>
<p><br><div class="loader"><img src="image/st1.jpg" alt="#" width=100% height=56.25%/></div>
<br><div><br><video width=100% height=56.25% controls><source src="image/ds.mp4" type="video/mp4">
</video></div></p>

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

</code></pre><p><b>switchState:</b> 
<br><br> An integer variable used to store the state of a switch connected to pin 7.
<br> 
<b>Function Definition:</b></p>
<p><b>readUltrasonicDistance(int triggerPin, int echoPin):</b> 
<br>A function that calculates the distance measured by an ultrasonic sensor. It takes two parameters: triggerPin for the trigger pin of the sensor and echoPin for the echo pin of the sensor. It returns the sound wave travel time in microseconds.
Setup Function:</p>
<p><b>setup():</b> This function runs once when the Arduino board is powered on or reset. It performs the following tasks:
Sets pin 9 and pin 10 as outputs to control external devices.
Sets pin 7 as an input to read the state of a switch.
Initializes the serial communication for debugging purposes.
Loop Function:</p>
<pre><code>&lt;b&gt;loop()<span class="hljs-symbol">:&lt;/b&gt;</span>
</code></pre><p><br>This function runs repeatedly after the setup() function. It performs the following tasks:
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
<br></p>
<p><br></p>
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
<br><br>The Fan Control System is designed to optimize comfort and energy efficiency by dynamically adjusting fan speeds based on environmental conditions. <br>Utilizing temperature, the system intelligently regulates the fan&#39;s operation, ensuring optimal air circulation and cooling. <br>Users can set preferences or allow the system to autonomously respond to changes in the ambient environment. <br>This project is applicable for home automation, offices, and industrial settings, providing a smart and energy-conscious solution for maintaining a comfortable and well-ventilated environment.

<b>How to connect the components in the circuit:</b>

<b>Arduino Connections:</b>
<br><br>The temperature sensor is connected to analog pin A0.
<br>The motor is connected to digital pin 13.
<br>The red LED is connected to digital pin 12.
<br>The green LED is connected to digital pin 11.
<br>The LCD is connected to digital pins 2, 3, 4, 5, 6, and 7.
Once we have completed these connections, we have the components connected according to the code.

<br><b>Here is the result on the tinkercad.</b>

<br><div class="loader"><img src="image/ds1.jpg" alt="#" width=100% height=56.25%/></div>
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
<br>The code includes the necessary library, &quot;LiquidCrystal.h,&quot; which allows the Arduino to communicate with and control the LCD display.

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
<br>Prints &quot;Welcome, Gladiators!&quot; on the LCD display at first.
<br>Sets the pin modes for the motor and LEDs as outputs.
<br>Adds a 2-second delay before continuing.
<br>Clears the LCD display.
<br>Prints &quot;Temp= &quot; on the first row and &quot;Fan= &quot; on the second row of the LCD display.

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
<br>Updates the LCD display with the corresponding status (&quot;ON&quot; or &quot;OFF&quot;) at the specified position.

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
<h1 style="font-size:1.5vw"><span style="color:black">Project Title: Voice Controlled Switch Using Alexa and Arduino</span></h1>

<p><a href="https://www.instructables.com/Smart-Switch-1/">Source</a></p>
<p>The main aim of this project is to use sound sensor to control
switch (relay) to turn on or off the device.</p>
<p>List of materials</p>
<ol>
<li><p>12V Relay Module</p>
</li>
<li><p>Arduino uno</p>
</li>
<li><p>DHT11 temperature sensor </p>
</li>
<li>ESP8266 Module </li>
<li><p>N26 optocoupler </p>
</li>
<li><p>LM1117 voltage regulator </p>
</li>
<li><p>Breadboard </p>
</li>
<li><p>Jumper wires </p>
</li>
<li><p>Push button </p>
</li>
</ol>
<p>This project is divided in three parts . First, heroku is applied to create an app . Second,Amazon Alexa is built to implement our work (Most importantpart). Third, Hardware is setup and programming is done using Arduino IDE.</p>
<p><br><div class="loader"><img src="image/image1a.png" alt="#" width=100% height=56.25%/></div>
<br></p>
<h1 id="step-1-linking-heroku-with-github">Step 1: Linking Heroku With GitHub</h1>
<p>Heroku is a cloud platform as a service (PaaS) supporting several programming languages that is used as a web application deployment model. First, go to heroku site create a new account or login there. Link is given below</p>
<p><a href="https://www.heroku.com/">Heroku Website</a></p>
<p>Let us start with creating a new app. App name is given
\&quot;iottempswitch\&quot; when you deploy app, link is generated.</p>
<p>Once app is made go to GitHub. <a href="https://github.com/">GitHub</a></p>
<p>Log in or sign up and create a new repository on GitHub. Choose a name and click &quot;Create repository.&quot;
On the next page, click on README and provide a description. Commit the new file.
Click the &quot;Upload&quot; button and either drag and drop files or choose them. Commit changes.
Open the Heroku app, go to the deploy section, and click on GitHub.
Enter the GitHub repository name (e.g., Smart-Relay). Copy and paste it, then click &quot;Connect.&quot;
Click &quot;Deploy branch (manual).&quot; Once deployed, find the link in the build log or settings for later use in creating the Amazon skill.</p>
<p><br><div class="loader"><img src="image/image2a.png" alt="#" width=100% height=56.25%/></div>
<br>
<br><div class="loader"><img src="image/image3a.png" alt="#" width=100% height=56.25%/></div>
<br>
<br><div class="loader"><img src="image/image4a.png" alt="#" width=100% height=56.25%/></div>
<br>
<br><div class="loader"><img src="image/image5a.png" alt="#" width=100% height=56.25%/></div>
<br>
<br><div class="loader"><img src="image/image6a.png" alt="#" width=100% height=56.25%/></div>
<br>
<br><div class="loader"><img src="image/image7a.png" alt="#" width=100% height=56.25%/></div>
<br></p>
<p><br><div class="loader"><img src="image/image8a.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image9a.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image10a.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image11.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image12.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image13.png" alt="#" width=100% height=56.25%/></div>
<br>
<br><div class="loader"><img src="image/image14.png" alt="#" width=100% height=56.25%/></div>
<br>
<br><div class="loader"><img src="image/image15.png" alt="#" width=100% height=56.25%/></div>
<br></p>
<h1 id="step-2-amazon">Step 2: Amazon</h1>
<p>Amazon service is used to control switch trigger by setting temperature and humidity on Amazon Developer site.</p>
<p>Go to Amazon Developer Site. Link is for <a href="https://developer.amazon.com/">Amazon Developer Website</a></p>
<p>Go to Developer console on top right as shown in figure i4</p>
<p>Go to Alexa then select Alexa Skill Kit and then create new skill by clicking on Add new skill</p>
<p>When you add new service you will see skill information page.</p>
<ol>
<li>Skill Information </li>
</ol>
<p>we have to provide skill type,language,name,invocation name.</p>
<p>Skill type ==\  select custom.</p>
<p>Name ==\  select any name.</p>
<p>Invocation name ==\  which you use while communicating with Alexa.For example ;- Alexa, ask sensor to turn switch trigger on or Alexa, ask light on here invocation names are sensor and light. Language ==\ 
English(India) . Select according to your country</p>
<p>click save and then next.</p>
<ol>
<li>Interaction Model</li>
</ol>
<p>The instructions guide the user through the process of setting up a skill using a skill builder. The skill, named &quot;smartswitch,&quot; involves defining multiple slot types, mapping these slots to intent slots, and adding a sample utterance for voice interaction. The intent is likely designed to handle queries related to switching states, sensor values, and temperature scales.</p>
<p>{Switch_State} switch trigger</p>
<p>set switch trigger to {Numbers} degree {tmp_scale}</p>
<p>turn switch {Switch_State}</p>
<p>{query} switch {Switch_State}
{query} is the current
{Sensor_Values}</p>
<p>After this save model and build it. Wait for model to be build after that click on configuration.After building you will see message.</p>
<ol>
<li>Configuration</li>
</ol>
<p>Select HTTPS and add link which was generated while creating heroku app . In my case it is <a href="https://iottempswitch.herokuapp.com/">find</a> After adding link click on next as
shown in image i23.</p>
<ol>
<li>SSL certificate</li>
</ol>
<p>Select second option and click on next. skill is successfully created</p>
<p><br><div class="loader"><img src="image/image18.png" alt="#" width=100% height=56.25%/></div>
<br>
<br><div class="loader"><img src="image/image19.png" alt="#" width=100% height=56.25%/></div>
<br></p>
<p><br><div class="loader"><img src="image/image20.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image21.png" alt="#" width=100% height=56.25%/></div>
<br></p>
<p><br><div class="loader"><img src="image/image22.png" alt="#" width=100% height=56.25%/></div>
<br>
<br><div class="loader"><img src="image/image23.png" alt="#" width=100% height=56.25%/></div>
<br></p>
<p><br><div class="loader"><img src="image/image24.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image25.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image26.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image27.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image28.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image29.png" alt="#" width=100% height=56.25%/>&lt;/div</p>
<p><br></p>
<p><br><div class="loader"><img src="image/image30.png" alt="#" width=100% height=56.25%/></div>
<br>
<br><div class="loader"><img src="image/image31.png" alt="#" width=100% height=56.25%/></div>
<br>
<br><div class="loader"><img src="image/image32.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image33.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image4.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image35.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image36.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image37.png" alt="#" width=100% height=56.25%/></div>
<br></p>
<p><br><div class="loader"><img src="image/image38.png" alt="#" width=100% height=56.25%/></div>
<br></p>
<h1 id="step-3-arduino">Step 3: Arduino</h1>
<p>Open Arduino IDE.Then go to File ==\  Preference.</p>
<p>In Addition Boards Manager, copy and paste the URL and click ok.</p>
<p>(URL(http://arduino.esp8266.com/stable/package_esp8266com_index.json)
Open Board Manager by going to Tools ==\  Board ==\ 
Board Manager. Open Boards Manager and search for nodemcu.
After that download ESP8266WiFi library.
Open library Manager : Sketch ==\  Include library ==\  Manage Libraries. 
Search for ESP8266WiFi library and install it.
Select board ==\  Generic ESP8266 Module. Before uploading the code we need
three libraries. Required libraries</p>
<p>Move this libraries to libraries folder of Arduino. You have to change three things in code SSID , PWD and your heroku app link. After that upload the code. For ESP Module you have to press flash button while uploading the code and then press reset button one time and then release the flash button. After uploading the code, open the terminal. you will see output.
<br><div class="loader"><img src="image/image41.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image42.png" alt="#" width=100% height=56.25%/></div>
<br></p>
<p><br><div class="loader"><img src="image/image43.png" alt="#" width=100% height=56.25%/></div>
<br></p>
<h1 id="step-4-component-description">Step 4: Component Description</h1>
<ol>
<li>What is a Relay</li>
</ol>
<p>relays act as intermediaries, allowing the safe and controlled interaction between circuits operating at different voltage levels. This makes them valuable components in various electrical and electronic applications, enhancing safety and functionality in circuit design.</p>
<p>How it works</p>
<p>A relay switch comprises two sections: input and output. The input has a coil energized by a small operating voltage. Output consists of contactors, including normally open (NO), normally closed (NC), and common (COM). Relay configurations like SPST, SPDT, and DPDT offer different contact combinations for switching circuits. The COM terminal is common, and if the coil receives rated voltage, COM and NO have continuity. The NC terminal powers on even without sufficient voltage. The NO terminal activates the output when the relay gets its rated voltage. Overall, relays facilitate controlled electrical switching.</p>
<ol>
<li>DHT temperature sensor</li>
</ol>
<p>The DHT11, a low-cost Humidity and Temperature Sensor, produces calibrated digital output. It seamlessly interfaces with microcontrollers like Arduino and Raspberry Pi, offering instantaneous and reliable results with long-term stability.</p>
<ol>
<li>ESP8266 Description</li>
</ol>
<p>The ESP8266 WiFi Module is a self-contained SOC with integrated TCP/IP, offering WiFi access to any microcontroller. It supports APSD for VoIP, Bluetooth co-existence, and has a self-calibrated RF, requiring no external parts.</p>
<p>Wi-Fi Direct (P2P),</p>
<p>soft-APIntegrated TCP/IP protocol
stack</p>
<p>Integrated TR switch, balun, LNA,
power amplifier and matching network</p>
<p>Integrated PLLs, regulators, DCXO and
power management units</p>
<p>+19.5dBm output power in 802.11b mode</p>
<p>Power down leakage current of \&lt;10uA</p>
<p>1MB Flash Memory</p>
<p>Integrated low power 32-bit CPU could
be used as application processor
SDIO 1.1 / 2.0, SPI, UART</p>
<p>STBC, 1×1 MIMO, 2×1 MIMOA-MPDU &amp;
A-MSDU aggregation &amp; 0.4ms guard interval</p>
<p>Wake up and transmit packets in \&lt;
2ms</p>
<p>Standby power consumption of \&lt; 1.0mW
(DTIM3)</p>
<p>Pin Description as shown in image i34. For connecting ESP Module with Arduino UNO we need Lm1117 3.3 voltage regulator or any regulator because Arduino is not capable of providing 3.3 v to ESP8266.</p>
<p><img src="media/image46.png" alt="">
<img src="media/image47.png" alt=""></p>
<p><img src="media/image50.png" alt=""><img src="media/image51.png" alt="">
<img src="media/image52.png" alt=""></p>
<h1 id="step-5-connections">Step 5: Connections</h1>
<p>ESP8266 === \  DHT11</p>
<p>GPIO0 === \  Output pin</p>
<p>ESP8266 === \  Relay</p>
<p>GPIO2 ===\  Input</p>
<p>ARDUINO ==\ ESP8266</p>
<p>Gnd ===\ Gnd TX === \  TX</p>
<p>RX === \  RX</p>
<p>Reset Button === \  RST Flash Button === \  GPIO0</p>
<h1 id="step-6-checking-all-the-things">Step 6: Checking All the Things</h1>
<p>App, skill, and hardware are ready. Ensure the ESP8266 is powered on as our server runs on it. While no sensor is connected, check connectivity by going to the Amazon skill&#39;s test page. Once verified, connect a sensor to the ESP8266. If used without ESP8266 connection, an error occurs. Utterance for testing.</p>
<p>set switch trigger to {Numbers} percent {tmp_scale}</p>
<p>ex :- set switch trigger to 50 percent humidity</p>
<p>{query} is the switch state</p>
<p>ex- on/off is the switch state</p>
<p>{Switch_State} switch trigger</p>
<p>ex -on/off switch trigger</p>
<p>set switch trigger to {Numbers}
degree {tmp_scale}</p>
<p>ex - set switch trigger to 76 degree fahrenheit ex - set switch
trigger to 24 degree celcius</p>
<p>turn switch {Switch_State}</p>
<p>ex - turn switch on/off</p>
<p>Alexa, ask arduino to turn switch trigger on/off</p>
<p>Alexa, ask arduino to set switch trigger to 24 degree celsius. Alexa,
ask arduino to set switch trigger to 50 percent humidity Alexa, ask
arduino to turn switch on/off</p>
<p><br><div class="loader"><img src="image/image53.png" alt="#" width=100% height=56.25%/></div>
<br>
<br><div class="loader"><img src="image/image54.png" alt="#" width=100% height=56.25%/></div>
<br></p>
<p><br><div class="loader"><img src="image/image55.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image56.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image57.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image58.png" alt="#" width=100% height=56.25%/></div>
<br></p>
<p><br><div class="loader"><img src="image/image60.png" alt="#" width=100% height=56.25%/></div>
<br></p>
<h1 id="step-7-vui-voice-user-interface-diagram">Step 7: VUI(Voice User Interface) Diagram</h1>
<p><br><div class="loader"><img src="image/image59.png" alt="#" width=100% height=56.25%/></div>
<br></p>
<h1 id="step-8-demo">Step 8: Demo</h1>
<p><video width=100% height=56.25% controls><source src="image/demo.mp4" type="video/mp4">
</video></p>
<ol>
<li><p>Set trigger for temperature and humidity.</p>
</li>
<li><p>Set trigger to 20 degree celsius.</p>
</li>
<li><p>Set trigger to 80 percent humidity.</p>
</li>
</ol>
<h1 id="step-9-schematic-diagram">Step 9: Schematic Diagram</h1>
<p><br><div class="loader"><img src="image/image61.png" alt="#" width=100% height=56.25%/></div>
<br><div class="loader"><img src="image/image62.png" alt="#" width=100% height=56.25%/></div></p>


