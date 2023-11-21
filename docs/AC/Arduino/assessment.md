  <h1 style="font-size:2vw"><span style="color:black">Introduction to Arduino</span></h1>
Arduino is a prototyping platform (open source) based on easy-to-use hardware and software. It consists of a programmable circuit board called a microcontroller and off-the-shelf software called the Arduino IDE (Integrated Development Environment) for writing and uploading computer code to the physical board.
<h1 style="font-size:1.5vw"><span style="color:black">The main features are:</span></h1>
The Arduino board is able to read analog or digital input signals from different sensors and convert them into outputs such as activating motors, turning on/off LEDs, connecting to the cloud and many other operations.

You can control board functions by sending a set of instructions to the microcontroller on the board through the Arduino IDE (upload software for short).

Unlike most previous programmable circuit boards, Arduino does not require additional hardware (called a programmer) to load new code onto the board. You just use a USB cable.

Additionally, the Arduino IDE uses a simplified version of C++, making it easier to learn programming.

Finally, Arduino offers a standard form factor that breaks the functionality of a microcontroller into easier-to-use packages
<h1 style="font-size:1vw"><span style="color:black">Types of Arduino boards</span></h1>

Various Arduino boards are available, depending on the microcontroller used. However, all Arduino boards have one thing in common: they are programmed through the Arduino IDE.

The differences are based on the number of inputs and outputs (number of sensors, LEDs, and buttons that can be used on a single board), speed, operating voltage, form factor, etc. Some boards are designed to be embedded and do not have a programming interface (hardware), so you will need to purchase them separately. Some can run directly from a 3.7V battery; others require at least 5V.

Below is a list of the different Arduino boards available.
<h1 style="font-size:1vw"><span style="color:black">Some Boards are</span></h1>

<link rel="stylesheet" href="css/bootstrap-grid.min.css"/>
<div class="demo">
        <div class="container">
            <div class="row text-center">
                <h1 class="white"></h1>
            </div>

<div class="row">
                <div class="col-md-4 col-sm-6">
                    <div class="arduino">
                        <div class="pic">
                            <img src="image/ar3.jpg">
                            <ul class="social">
                                <li><a href="https://store.arduino.cc/products/arduino-uno-rev3" class="fab fa-facebook">Arduino UNO R3</a></li>
                            </ul>
                        </div>
                        <div class="team-content">
                            <h3 class="title"></h3>
                            <h3><a href="https://store.arduino.cc/products/arduino-uno-rev3" class="title"></a></h3>
                        </div>
                    </div>
                </div>

<div class="col-md-4 col-sm-6">
                    <div class="arduino">
                        <div class="pic">
                            <img src="image/ar4.jpg">
                            <ul class="social">
                                <li><a href="https://store.arduino.cc/products/arduino-mega-2560-rev3" class="fab fa-facebook">Arduino Mega 2560 Rev3</a></li>
                            </ul>
                        </div>
                    </div>
                </div>

<div class="col-md-4 col-sm-6">
                    <div class="arduino">
                        <div class="pic">
                            <img src="image/ar5.jpg">
                            <ul class="social">
                                <li><a href="https://store.arduino.cc/products/arduino-leonardo-with-headers" class="fab fa-facebook">Arduino Leonardo</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
            


<div class="col-md-4 col-sm-6">
                    <div class="arduino">
                        <div class="pic">
                            <img src="image/ar6.jpg">
                            <ul class="social">
                                <li><a href="https://store.arduino.cc/products/arduino-uno-wifi-rev2" class="fab fa-facebook">Arduino UNO WiFi Rev2</a></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>

<br><h1 style="font-size:1.5vw"><span style="color:black">Arduino Installation</span></h1>

Here is a simple steps how to set up the Arduino IDE on our computer and prepare the board to receive the program via USB cable.

<br><h1 style="font-size:1.5vw"><span style="color:black">Step 1 </span></h1>
 First, you must have Arduino board (you can choose the one you like) and a USB cable. If you use an Arduino UNO, Arduino Duemilanove, Nano, Arduino Mega 2560 or De="coliecimila, you will need a standard USB cable (A plug to B plug). The picture below shows the type of USB printer you will connect to.
 <br><div class="loader"><img src="image/ar.jpg" alt="#" /></div>

<br><h1 style="font-size:1vw"><span stylor:black">Step 2 - Download the Arduino IDE software.</span></h1>

Downloading the Arduino IDE software is the first step in getting started with Arduino programming. Here's a step-by-step guide on how to download the Arduino IDE:

<br><h1 style="font-size:1.5vw"><span style="color:black">A. Visit the Arduino Software Download Page:</span></h1>
Go to the official Arduino website's software download page: [Arduino Software](https://www.arduino.cc)
<br><h1 style="font-size:1.5vw"><span style="color:black">B. Choose Your Operating System::</span></h1>
On the download page, you'll see options for different operating systems, such as Windows, Mac OS X, and Linux. Select the version that corresponds to your computer's operating system.
<br><h1 style="font-size:1.5vw"><span style="color:black">C. Download the Installer:</span></h1>
Click on the download [download](https://support.arduino.cc/hc/en-us/articles/360019833020-Download-and-install-Arduino-IDE).link for your chosen operating system. This will typically download an installer file to your computer.
<br><h1 style="font-size:1.5vw"><span style="color:black">D. Install the Arduino IDE:</span></h1>
Once the download is complete, locate the installer file and run it to start the installation process.
Follow the on-screen instructions to install the Arduino IDE on your computer.
<br><h1 style="font-size:1.5vw"><span style="color:black">E. Launch the Arduino IDE:</span></h1>
After the installation is complete, you can launch the Arduino IDE. The IDE should be accessible from your computer's applications or programs menu.
<br><div class="loader"><img src="image/1.jpg" alt="#" /></div>
<br><h1 style="font-size:1.5vw"><span style="color:black">F. Select the Board and Port:</span></h1>
Before uploading your sketches to an Arduino board, make sure to select the correct board and port in the Arduino IDE. You can do this by going to the Tools menu and choosing the appropriate options.
<br><div class="loader"><img src="image/3.jpg" alt="#" /></div>
<br><h1 style="font-size:1.5vw"><span style="color:black">F. Check for Updates:</span></h1>
Periodically, it's a good idea to check for updates to the Arduino IDE. You can do this by going to the Arduino IDE's Help menu and selecting the "Check for Updates" option.
Creating a new sketch in the Arduino IDE is the initial step in starting a new Arduino project. 
<br><h1 style="font-size:1.5vw"><span style="color:black">A. Open the Arduino IDE:</span></h1>
Launch the Arduino IDE on your computer. After a successful installation, you can typically find the Arduino IDE in your applications or programs menu.
<br><h1 style="font-size:1.5vw"><span style="color:black">B. Access the Sketch Menu::</span></h1>
Once the Arduino IDE is open, you'll see a menu bar at the top. Click on the "File" menu.
Select "New":
In the "File" menu, hover your mouse over "New" to reveal a sub-menu. From there, click on "New" again. Alternatively, you can use the keyboard shortcut Ctrl + N (Windows/Linux) or Cmd + N (Mac) to create a new sketch.
<br><h1 style="font-size:1.5vw"><span style="color:black">C. New Sketch Window:</span></h1>
After selecting "New," a new window will open, providing a blank canvas for your Arduino sketch. This window is where you'll write your code.
<br><div class="loader"><img src="image/2.jpg" alt="#" /></div>
<br><h1 style="font-size:1.5vw"><span style="color:black">D. Understand the Default Template:</span></h1>
The new sketch window comes with a default template that includes two essential functions: setup() and loop(). These functions are the starting points for your code.

<br><b>The setup() function:</b> is called once when the Arduino starts. It's used for initializing variables, setting pin modes, and other setup tasks.

<br><b>The loop() function:</b>The loop() function is where your main code goes. It runs continuously in a loop after the setup() function finishes.

<br>Here's the default template:
<br><div class="loader"><img src="image/4.jpg" alt="#" /></div>
<br><h1 style="font-size:1.5vw"><span style="color:black">E. Save Your Sketch:</span></h1>
Before you start writing your code, it's a good practice to save your sketch. Click on the "File" menu and select "Save" or use the keyboard shortcut Ctrl + S (Windows/Linux) or Cmd + S (Mac). Choose a location on your computer and give your sketch a meaningful name.
<br><h1 style="font-size:1.5vw"><span style="color:black">F.Write Your Code:</span></h1>
Now, you're ready to write your Arduino code within the setup() and loop() functions. Add the specific instructions and logic for your project.
<br><h1 style="font-size:1.5vw"><span style="color:black">G.Verify/Compile Your Sketch:</span></h1>
To check for syntax errors and compile your sketch, click the checkmark icon in the toolbar or go to Sketch > Verify/Compile. The IDE will display any errors in the console at the bottom of the window.
<br><h1 style="font-size:1.5vw"><span style="color:black">H.Upload Your Sketch:</span></h1>
If there are no errors, you can proceed to upload your sketch to the Arduino board. Connect your Arduino board to your computer, select the correct board and port from the Tools menu, and click the right arrow icon in the toolbar or go to Sketch > Upload.
<br><h1 style="font-size:1.5vw"><span style="color:black">I.Monitor Serial Output:</span></h1>
If your sketch uses the Serial library for communication, you can open the Serial Monitor (Tools > Serial Monitor) to view messages from your Arduino.
<br><h1 style="font-size:1.5vw"><span style="color:black">J.Debug and Iterate:</span></h1>
If needed, use the Serial Monitor and the IDE's built-in tools for debugging. Modify your code as necessary and repeat the verification and upload process.

<br>The above descriptions are the key features of IDE We use to do a simple project. However, Each section can be described as follows in detail.
<h1 style="font-size:1.5vw"><span style="color:black">EDIT:</span></h1>

<strong>Undo (Ctrl + Z):</strong></b>
The "Undo" feature allows you to revert the last action you performed. It's useful when you make a mistake or want to go back to a previous state of your code.

<b><strong>Redo (Ctrl + Y):</strong></b>
The "Redo" feature is the opposite of "Undo." It allows you to reapply an action that you previously undid.

<b><strong>Cut (Ctrl + X):</strong></b> 
"Cut" is used to remove the selected text or code and place it in the clipboard. You can then use the "Paste" feature to insert it elsewhere.

<b><strong>Copy (Ctrl + C):</strong></b> 
"Copy" allows you to duplicate the selected text or code and place it in the clipboard. You can then use the "Paste" feature to insert it elsewhere.

<b><strong>Paste (Ctrl + V):</strong></b>
"Paste" is used to insert the content from the clipboard at the current cursor position. This is handy for copying and moving code within your sketch.

<b><strong>Select All (Ctrl + A):</strong></b>
"Select All" highlights and selects the entire content of the currently active window. This is useful when you want to perform an action on the entire code.

<b><strong>Find (Ctrl + F):</strong></b> 
The "Find" feature allows you to search for a specific word or string within your code. It opens a small dialog where you can enter the text you want to find.

<b><strong>Find Next (ctrl+G):</strong></b> 
"Find Next" is used to continue searching for the next occurrence of the text specified in the "Find" feature.

<b><strong>Find Previous (ctrl+shift+G):</strong></b> 
"Find Previous" is used to search for the previous occurrence of the text specified in the "Find" feature.

<b><strong>Replace (Ctrl + H):</strong></b> 
"Replace" allows you to search for a specific word or string and replace it with another. It opens a dialog where you can enter both the search and replacement text.

<b><strong>Go to Line (Ctrl + G):</strong></b> 
"Go to Line" allows you to jump to a specific line number in your code. It's useful for quickly navigating to a particular section of your sketch.

<b><strong>Toggle Comment (Ctrl + /):</strong></b>
"Toggle Comment" is used to comment or uncomment selected lines of code. Comments are non-executable lines that you can use to add notes or explanations to your code.

<b><strong>Increase Indent (Ctrl + ]):</strong></b>
"Increase Indent" is used to increase the indentation of the selected code. Proper indentation enhances code readability.

<b><strong>Decrease Indent (Ctrl + [):</strong></b> 
"Decrease Indent" is used to decrease the indentation of the selected code.

<br><b><strong> Auto Format (Ctrl + T):</strong></b>
"Auto Format" automatically formats your code according to the defined coding style. It helps maintain a consistent and readable code structure.

<h1 style="font-size:1.5vw"><span style="color:black">SKETCH:</span></h1>
<b><strong>Verify/Compile (Ctrl + R):</strong></b> 
This option compiles your Arduino sketch, checking for syntax errors. It ensures that your code is correctly written and ready for uploading to the Arduino board.

<b><strong>Upload (Ctrl + U):</strong></b>
The "Upload" option is used to upload your compiled sketch to the connected Arduino board. This makes your code executable on the hardware.

<b><strong>Export Compiled Binary:</strong></b>
This option allows you to export the compiled binary (.hex) file of your sketch. This file can be useful for sharing or archiving your compiled code without sharing the entire sketch.

<b><strong>Show Sketch Folder (Ctrl + K):</strong></b>
Opens the folder where your current Arduino sketch is stored on your computer. This is useful for managing additional files associated with your project.

<b><strong>Include Library:</strong></b>
This submenu provides options for managing libraries in your sketch. You can include additional libraries that provide pre-written code for various functions.

<b><strong>Manage Libraries:</strong></b>
Opens the Library Manager, allowing you to browse and install libraries from the Arduino Library Repository.
<b><strong>Import Library:</strong></b>
Allows you to import a custom library into your Arduino sketch.

<b><strong>Add File:</strong></b>
Adds an additional file to your sketch. This can be useful for organizing your code into multiple files for larger projects.

<b><strong>New Tab (Ctrl + T):</strong></b>
Adds a new tab to your Arduino sketch. Tabs can be used to organize your code into separate sections or files.

<b><strong>Close:</strong></b>
Closes the current sketch.

<b><strong>Save (Ctrl + S):</strong></b>
 Saves the current sketch.
<b><strong>Save As(Ctrl + shift + S):</strong></b>
Saves the current sketch with a new name or in a different location.

<b><strong>Revert to Saved:</strong></b>
Reverts the sketch to the last saved state.
<br><h1 style="font-size:1.5vw"><span style="color:black">TOOLS:</span></h1>
<b><strong>Board:</strong></b>
This submenu allows you to select the type of Arduino board you are using for your project. It includes a list of supported Arduino boards and third-party boards. Selecting the correct board is essential for compiling and uploading your sketch to the right hardware.

<b><strong>Port:</strong></b>
The "Port" submenu is used to select the communication port to which your Arduino board is connected. This option is crucial for uploading your sketch to the correct Arduino board.

<b><strong>Programmer:</strong></b>
If you are using a different programming method or a custom programmer, you can select it from this submenu.

<b><strong>Boards Manager:</strong></b>
Opens the Boards Manager, where you can add support for additional Arduino boards. This is useful when working with non-standard or third-party Arduino-compatible boards.

<b><strong>Port Monitor (Ctrl + Shift + M):</strong></b>
Opens the Serial Monitor, which allows you to communicate with your Arduino board via the serial interface. This is useful for debugging and monitoring output from your Arduino sketch.

<b><strong>Auto Format (Ctrl + T):</strong></b>
Automatically formats your code according to the defined coding style. It helps maintain a consistent and readable code structure.

<b><strong>Serial Plotter:</strong></b>
Opens the Serial Plotter, a tool for visualizing data sent from your Arduino board over the serial port. This is useful for plotting sensor data, monitoring values, and more.

<b><strong>Create a Library:</strong></b>
Opens the Library Creator, a tool that helps you create your own libraries for use in Arduino sketches.

<b><strong>Programmer:</strong></b>
Allows you to select a specific programmer for burning the bootloader or uploading code to the Arduino board.

<b><strong>Burn Bootloader:</strong></b>
Initiates the process of burning the bootloader onto an Arduino board, which is necessary when setting up certain types of boards or recovering from issues.
<br><h1 style="font-size:1.5vw"><span style="color:black">Help:</span></h1>
The "Help" menu in the Arduino IDE provides access to various resources and tools that can assist you in using the IDE, programming Arduino boards, and troubleshooting issues. Here's an overview of the options you'll typically find in the "Help" menu:

<b><strong>Getting Started:</strong></b>
This option usually opens a web browser and directs you to the official Arduino website's "Getting Started" guide. It's a resource for beginners to understand the basics of Arduino and the IDE.

<b><strong>Examples:</strong></b>
Opens a submenu with a list of example sketches that come bundled with the Arduino IDE. These examples cover a variety of basic and advanced topics to help you learn how to use different Arduino features.

<b><strong>Reference:</strong></b>
Opens a web browser and takes you to the official Arduino reference documentation. This documentation provides detailed information about the Arduino programming language, functions, and libraries.

<b><strong>Updates:</strong></b>
Checks for updates to the Arduino IDE. If a new version is available, you can download and install it from this menu.

<b><strong>About Arduino:</strong></b>

Displays information about the current version of the Arduino IDE, including the version number and copyright details.

<h1 style="font-size:1.2vw"><span style="color:black">TinkerCAD</span></h1>
Tinkercad is an online platform that provides a virtual environment for designing, simulating, and creating electronic circuits and 3D models. It is widely used by hobbyists, students, and professionals to prototype and test their ideas without the need for physical components or equipment.

<h1 style="font-size:1.2vw"><span style="color:black">Key features and capabilities of Tinkercad include:</span></h1>

<b><strong>Circuit Design:</strong></b>  Tinkercad offers a user-friendly interface for designing electronic circuits using a wide range of components such as resistors, capacitors, LEDs, sensors, microcontrollers, and more. Users can drag and drop components onto the workspace, connect them using virtual wires, and simulate the behavior of the circuit.

<b><strong>Code Simulation:</strong></b> Tinkercad supports programming and code simulation for microcontrollers like Arduino. Users can write code in a built-in code editor, upload it to the virtual microcontroller, and visualize the behavior of the circuit based on the code logic.

<b><strong>Collaboration and Sharing:</strong></b> Tinkercad enables users to collaborate on projects by inviting others to view and edit their designs. It supports real-time collaboration and provides sharing options to showcase designs publicly or privately.

<b><strong>Learning Resources:</strong></b> Tinkercad offers various tutorials, lessons, and projects to help users learn and explore electronics and 3D design. It caters to beginners with step-by-step instructions and gradually introduces more advanced concepts.

<b><strong>Integration with Arduino:</strong></b> Tinkercad has a seamless integration with the Arduino platform, making it easy to design circuits and simulate Arduino-based projects. It supports a wide range of Arduino boards and provides a simulated environment to test and debug code.

<h1 style="font-size:1.2vw"><span style="color:black">Steps to Access Tinkercad :</span></h1>

<b><strong>Open a web browser:</strong></b> Launch your preferred web browser on your computer or mobile device.

<b><strong>Go to the Tinkercad website:</strong></b> Click This [tinkercad.com](https://www.tinkercad.com/.)

<b><strong>Sign in or create an account:</strong></b> If you already have a Tinkercad account, click on the "Sign In" button and enter your login credentials (email and password). If you don't have an account, click on the "Join Now" button to create a new account. You can sign up using your email address or by linking your Google, Facebook, or Autodesk account.
<br><div class="loader"><img src="image/tin.jpg" alt="#" /></div>
<br><br>

<b><strong>Explore the Tinkercad interface:</strong></b>  Once you are signed in, you will be taken to the Tinkercad workspace. The interface consists of different sections, including the Circuit Design, Code Editor, and 3D Design areas. Take a moment to familiarize yourself with the layout and tools available.
<br><div class="loader"><img src="image/tin1.jpg" alt="#" /></div>

<b><strong>Choose your design area:</strong></b> You can select the Circuit Design area by clicking on the corresponding tab at the top of the workspace. The Circuit Design area is for creating electronic circuits.
<br><div class="loader"><img src="image/tin2.jpg" alt="#" /></div>

<b><strong>Start creating:</strong></b> Begin by dragging and dropping components onto the workspace in the Circuit Design area. Connect components with virtual wires in the Circuit Design area 
<br><div class="loader"><img src="image/tin3.jpg" alt="#" /></div>

<b><strong>Simulate and test:</strong></b>clicking on the "Start Simulation" button. You can also write and upload code to microcontrollers like Arduino in the Code Editor area.
<br><div class="loader"><img src="image/tin4.jpg" alt="#" /></div>

Save and share your designs: Once you have created your circuits, you can save them by clicking on the "Save" button. You can also share your designs with others by clicking on the "Send to" button and providing the necessary permissions.
<br><div class="loader"><img src="image/tin5.jpg" alt="#" /></div>

<h1 style="font-size:1.2vw"><span style="color:black">Reference</span></h1>

- [Nexmaker](https://www.nexmaker.com/doc/9IOT/NodeMCUESP8266_ALiYun.html)
- [tinkercad](https://www.tinkercad.com/.)
- [Javatpoints](https://www.javatpoint.com/arduino)

<h1 style="font-size:1vw"><span style="color:black">Arduino input</span></h1>
We can use swith to control the circuit, in this case we use pin 7 as input port

<br><div class="loader"><img src="image/switch.png" alt="#" /></div>
<br>
<h1 style="font-size:1vw"><span style="color:black"></span>Switch</h1>
<br>


```html
const int LED1=12;
const int LED2=13;
int val=0;
void setup()
{ 
  pinMode(LED1, OUTPUT); 
  pinMode(LED2, OUTPUT);
  pinMode(7, INPUT);
  void loop (){
    val=digitalRead(7);
    if(val==HIGH)
    {
      digitalWrite(LED1,HIGH);
      digitalWrite(LED2,LOW);
    }
    else
    {
      digitalWrite(LED2,HIGH);
      digitalWrite(LED1,LOW);
    }
    delay(1000);
  }
}
```
<b>Here is line by line discription:</b>

    const int LED1 = 12;
    const int LED2 = 13;
    int val = 0;
This declares two constants, LED1 and LED2, with values 12 and 13 respectively. These constants represent the pin numbers of two LEDs.
the last variable declares an integer variable val and initializes it to 0.

    void setup()
    { 
    pinMode(LED1, OUTPUT); pin refers the firt coordinate whereas Mode points the second coordinate
    pinMode(LED2, OUTPUT);
    pinMode(7, INPUT);}
Begins the setup() function, which is a standard Arduino function that is called once when the microcontroller starts.
Sets LED1 and LED2 pins as output using pinMode() function.
Sets pin 7 as an input pin using pinMode() function.

    void loop (){
        val = digitalRead(7);
        if (val == HIGH)
        {
        digitalWrite(LED1, HIGH);
        digitalWrite(LED2, LOW);
        }
        else
        {
        digitalWrite(LED2, HIGH);
        digitalWrite(LED1, LOW);
        }
        delay(1000);
    }
Begins the loop() function, which is a standard Arduino function that runs repeatedly after the setup() function.
Reads the value from pin 7 and stores it in the val variable using the digitalRead() function.
Checks if val is equal to HIGH.
If true, it turns on LED1 by setting its pin to HIGH and turns off LED2 by setting its pin to LOW.
If false, it turns on LED2 by setting its pin to HIGH and turns off LED1 by setting its pin to LOW.
Delays the execution of the code for 1000 milliseconds (1 second) using the delay() function.
<br>


<h1 style="font-size:1vw"><span style="color:black">Ultrasonic Distance sensor</span></h1>
ultrasonic sensors measure distance by using ultrasonic waves. The sensor head emits an ultrasonic wave and receives the wave reflected back from the target. Ultrasonic Sensors measure the distance to the target by measuring the time between the emission and reception. 
<video width="320" height="240" controls>
  <source src="image/ulds.mp4" type="video/mp4">
</video>
<br>Material used are:

    - 1 Arduino Uno
    - 1 Breadboard
    - 1 Ultrasonic Distance Sensor
    - 3 LEDs
    - 3 Resistors (220ohms)


        ```
        int distanceThreshold = 0;

        int cm = 0;

        int inches = 0;

        long readUltrasonicDistance(int triggerPin, int echoPin)
        {
        pinMode(triggerPin, OUTPUT);  
        digitalWrite(triggerPin, LOW);
        delayMicroseconds(2);
        digitalWrite(triggerPin, HIGH);
        delayMicroseconds(10);
        digitalWrite(triggerPin, LOW);
        pinMode(echoPin, INPUT);
        return pulseIn(echoPin, HIGH);
        }

        void setup()
        {
        Serial.begin(9600);
        pinMode(2, OUTPUT);
        pinMode(3, OUTPUT);
        pinMode(4, OUTPUT);
        }

        void loop()
        {
        distanceThreshold = 35;
        cm = 0.01723 * readUltrasonicDistance(7, 6);
        inches = (cm / 2.54);
        Serial.print(cm);
        Serial.print("cm, ");
        Serial.print(inches);
        Serial.println("in");
        if (cm > distanceThreshold) {
            digitalWrite(2, LOW);
            digitalWrite(3, LOW);
            digitalWrite(4, LOW);
        }
        if (cm <= distanceThreshold && cm > distanceThreshold - 15) {
            digitalWrite(2, HIGH);
            digitalWrite(3, LOW);
            digitalWrite(4, LOW);
        }
        if (cm <= distanceThreshold - 15 && cm > distanceThreshold - 25) {
            digitalWrite(2, HIGH);
            digitalWrite(3, HIGH);
            digitalWrite(4, LOW);
        }
        if (cm <= distanceThreshold - 25 && cm > distanceThreshold - 35) {
            digitalWrite(2, HIGH);
            digitalWrite(3, HIGH);
            digitalWrite(4, HIGH);
        }
        if (cm <= distanceThreshold - 35) {
            digitalWrite(2, HIGH);
            digitalWrite(3, HIGH);
            digitalWrite(4, HIGH);
        }
        delay(100); // Wait for 100 millisecond(s)
        }
        ```
<b>Discription of the code:</b>
    int distanceThreshold = 0;
Declares an integer variable distanceThreshold and initializes it to 0.

    int cm = 0;
    int inches = 0;
Declares two integer variables cm and inches and initializes them to 0.

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
Defines a function named readUltrasonicDistance that takes two integer parameters: triggerPin and echoPin.
<br>Inside the function, it sets the triggerPin as an output pin, clears the trigger by setting it to low, waits for 2 microseconds, then sets the trigger pin to a high state for 10 microseconds before setting it back to low.
<br>It sets the echoPin as an input pin.
<br>It uses the pulseIn() function to read the echo pin and returns the sound wave travel time in microseconds.

    void setup()
    {
        Serial.begin(9600);
        pinMode(2, OUTPUT);
        pinMode(3, OUTPUT);
        pinMode(4, OUTPUT);
    }
<br>Begins the setup() function, which is a standard Arduino function that is called once when the microcontroller starts.
<br>Initializes the serial communication at a baud rate of 9600.
<br>Sets pins 2, 3, and 4 as output pins using the pinMode() function.

    void loop()
    {
        distanceThreshold = 35;
        cm = 0.01723 * readUltrasonicDistance(7, 6);
        inches = (cm / 2.54);
        Serial.print(cm);
        Serial.print("cm, ");
        Serial.print(inches);
        Serial.println("in");

        // Conditions to control the LEDs based on the measured distance
        if (cm > distanceThreshold) {
            digitalWrite(2, LOW);
            digitalWrite(3, LOW);
            digitalWrite(4, LOW);
        }
        if (cm <= distanceThreshold && cm > distanceThreshold - 15) {
            digitalWrite(2, HIGH);
            digitalWrite(3, LOW);
            digitalWrite(4, LOW);
        }
        if (cm <= distanceThreshold - 15 && cm > distanceThreshold - 25) {
            digitalWrite(2, HIGH);
            digitalWrite(3, HIGH);
            digitalWrite(4, LOW);
        }
        if (cm <= distanceThreshold - 25 && cm > distanceThreshold - 35) {
            digitalWrite(2, HIGH);
            digitalWrite(3, HIGH);
            digitalWrite(4, HIGH);
        }
        if (cm <= distanceThreshold - 35) {
            digitalWrite(2, HIGH);
            digitalWrite(3, HIGH);
            digitalWrite(4, HIGH);
        }
        delay(100);
    }
<br>Begins the loop() function, which is a standard Arduino function that runs repeatedly after the setup() function.
<br>Sets the distanceThreshold to 35.
<br>Calculates the distance in centimeters by calling the readUltrasonicDistance() function with trigger and echo pin numbers and multiplying the result by a conversion factor.
<br>Converts the distance to inches by dividing cm to 2.54.
<br>Prints the measured distance in centimeters and inches using the Serial.print() and Serial.println() functions.
<br>Controls the LEDs based on the measured distance:
<br>If the distance is greater than the distanceThreshold, turns off all LEDs.
<br>If the distance is less than or equal to distanceThreshold and greater than distanceThreshold - 15, turns on LED2 and turns off LED1 and LED3.
<br>If the distance is less than or equal to distanceThreshold - 15 and greater than distanceThreshold - 25, turns on LED2 and LED3 and turns off LED1.
<br>If the distance is less than or equal to distanceThreshold - 25 and greater than distanceThreshold - 35, turns on all LEDs (LED1, LED2, and LED3).
<br>If the distance is less than or equal to distanceThreshold - 35, turns on all LEDs (LED1, LED2, and LED3).
<>Delays the execution of the code for 100 milliseconds using the delay() function.

<h1 style="font-size:1vw"><span style="color:black">Temprature Sensor</span></h1>
<br><div class="loader"><img src="image/tms.jpg" alt="#" /></div>
A temperature sensor is a device used to measure temperature
<br>Material used are:

   - 1 Arduino Uno R3
   - 1 Resistors (4.7Kohms)
   - 1 Yellow LED
   - 1 Blue LED	
   - 1 Green LED
   - 3 1 kΩ Resistor
   - 1 Temperature Sensor [TMP36]
<h1 style="font-size:1vw"><span style="color:black">Code</span></h1>

        ```html
    int baselineTemp = 0;
    int celsius = 0;
    int fahrenheit = 0;

    void setup()
    {
    pinMode(A0, INPUT);
    Serial.begin(9600);

    pinMode(2, OUTPUT);
    pinMode(3, OUTPUT);
    pinMode(4, OUTPUT);
    }

    void loop()
    {
    baselineTemp = 40;
    
    celsius = map(((analogRead(A0) - 20) * 3.04), 0, 1023, -40, 125);
    
    fahrenheit = ((celsius * 9) / 5 + 32);
    Serial.print(celsius);
    Serial.print(" C, ");
    Serial.print(fahrenheit);
    Serial.println(" F");
    
    if (celsius < baselineTemp) {
        digitalWrite(2, LOW);
        digitalWrite(3, LOW);
        digitalWrite(4, LOW);
    }
    if (celsius >= baselineTemp && celsius < baselineTemp + 10) {
        digitalWrite(2, HIGH);
        digitalWrite(3, LOW);
        digitalWrite(4, LOW);
    }
    if (celsius >= baselineTemp + 10 && celsius < baselineTemp + 20) {
        digitalWrite(2, HIGH);
        digitalWrite(3, HIGH);
        digitalWrite(4, LOW);
    }
    if (celsius >= baselineTemp + 20 && celsius < baselineTemp + 30) {
        digitalWrite(2, HIGH);
        digitalWrite(3, HIGH);
        digitalWrite(4, HIGH);
    }
    if (celsius >= baselineTemp + 30) {
        digitalWrite(2, HIGH);
        digitalWrite(3, HIGH);
        digitalWrite(4, HIGH);
    }
    delay(1000); 
    }

<b>Descriptio of the code</b>
    int baselineTemp = 0;
    int celsius = 0;
    int fahrenheit = 0;
<br>Declares three integer variables: baselineTemp, celsius, and fahrenheit, and initializes them to 0. <br>These variables will be used to store the baseline temperature, the temperature in Celsius, and the temperature in Fahrenheit, respectively.
   
   void setup()
    {
        pinMode(A0, INPUT);
        Serial.begin(9600);

        pinMode(2, OUTPUT);
        pinMode(3, OUTPUT);
        pinMode(4, OUTPUT);
    }
<br>Begins the setup() function, which is a standard Arduino function that is called once when the microcontroller starts.
<br>Sets pin A0 as an input pin using the pinMode() function. This pin is used to read the analog temperature sensor.
<br>Initializes the serial communication at a baud rate of 9600.
<br>Sets pins 2, 3, and 4 as output pins using the pinMode() function. These pins will control the LEDs.

    void loop()
    {
        baselineTemp = 40;

        celsius = map(((analogRead(A0) - 20) * 3.04), 0, 1023, -40, 125);

        fahrenheit = ((celsius * 9) / 5 + 32);
        Serial.print(celsius);
        Serial.print(" C, ");
        Serial.print(fahrenheit);
        Serial.println(" F");

        if (celsius < baselineTemp) {
            digitalWrite(2, LOW);
            digitalWrite(3, LOW);
            digitalWrite(4, LOW);
        }
        if (celsius >= baselineTemp && celsius < baselineTemp + 10) {
            digitalWrite(2, HIGH);
            digitalWrite(3, LOW);
            digitalWrite(4, LOW);
        }
        if (celsius >= baselineTemp + 10 && celsius < baselineTemp + 20) {
            digitalWrite(2, HIGH);
            digitalWrite(3, HIGH);
            digitalWrite(4, LOW);
        }
        if (celsius >= baselineTemp + 20 && celsius < baselineTemp + 30) {
            digitalWrite(2, HIGH);
            digitalWrite(3, HIGH);
            digitalWrite(4, HIGH);
        }
        if (celsius >= baselineTemp + 30) {
            digitalWrite(2, HIGH);
            digitalWrite(3, HIGH);
            digitalWrite(4, HIGH);
        }
        delay(1000);
    }

<br>Begins the loop() function, which is a standard Arduino function that runs repeatedly after the setup() function.
<br>Sets the baselineTemp to 40. This variable represents the baseline temperature value.
<br>Reads the analog value from pin A0 using the analogRead() function and applies some mathematical calculations and mapping to convert it to temperature in Celsius. The formula used involves subtracting 20 from the reading, multiplying by 3.04, and mapping the result from the input range (0-1023) to the output range (-40 to 125).
<br>Converts the temperature in Celsius to Fahrenheit using the formula (celsius * 9) / 5 + 32.
<br>Prints the temperature in Celsius and Fahrenheit to the serial monitor using the Serial.print() and Serial.println() functions.
<br>Controls the LEDs based on the measured temperature:
<br>If the temperature is below the baselineTemp, turns off all LEDs.
<br>If the temperature is greater than or equal to baselineTemp and less than baselineTemp + 10, turns on LED2 and turns off LED1 and LED3.
<br>If the temperature is greater than or equal to baselineTemp + 10 and less than baselineTemp + 20, turns on LED2 and LED3 and turns off LED1.
<br>If the temperature is greater than or equal to baselineTemp + 20 and less than baselineTemp + 30, turns on all LEDs (LED1, LED2, and LED3).
<br>If the temperature is greater than or equal to baselineTemp + 30, turns on all LEDs (LED1, LED2, and LED3).
<br>Delays the execution of the code for 1000 milliseconds (1 second) using the delay() function. This controls the rate at which the temperature readings are obtained and displayed.
<br>

<br>
<h1 style="font-size:1vw"><span style="color:black">Arduino Output</span></h1>
<video width="320" height="240" controls>
  <source src="image/servo.mp4" type="video/mp4">
</video>
<h1 style="font-size:1vw"><span style="color:black">Serve Motor</span></h1>

<br>
A servomotor is a closed-loop servomechanism that uses position feedback to control its motion and final position

<br>Material used are:

   - 1 Arduino Uno R3
   - 1 Positional Micro Servo

<h1 style="font-size:1vw"><span style="color:black">Code</span></h1>



    // Incluimos la librería para Servo
    #include <Servo.h>

    Servo servoBase;//Asigno un nombre específico

    void setup() {
    servoBase.attach(A1);//Pin a utilizar para servo
    servoBase.write(0);  //asigno 0 al servo motor
    }

    void loop() {

    for(int i=0; i<=180; i=i+10)
    {
    servoBase.write(i);
    delay(2000);
    }
    }
    

    #include <Servo.h>
<br>This line includes the Servo library, which provides functions for controlling servo motors.

    Servo servoBase;
Declares a Servo object named servoBase. This object will be used to control the servo motor.
            ```
            void setup() {
        servoBase.attach(A1);
        servoBase.write(0);
        }
<br>The setup() function is a standard Arduino function that is called once when the microcontroller starts.
<br>Attaches the servo motor to pin A1 using the attach() function. This informs the Arduino that the servo motor will be connected to pin A1.
<br>Writes a value of 0 to the servo motor using the write() function. This sets the initial position of the servo motor to 0 degrees.

    void loop() {
    for (int i = 0; i <= 180; i = i + 10) {
        servoBase.write(i);
        delay(2000);
    }
    }
<br>The loop() function is a standard Arduino function that runs repeatedly after the setup() function.
<br>In this code, a for loop is used to control the servo motor. It starts with i initialized to 0 and increments i by 10 in each iteration until it reaches 180.
<br>Inside the loop, the write() function is used to set the position of the servo motor to the current value of i.
<br>The delay() function pauses the execution for 2000 milliseconds (2 seconds) before moving to the next iteration of the loop. This creates a delay between each position change, allowing time for the servo motor to move to the desired angle.


<h1 style="font-size:1vw"><span style="color:black">LED Display</span></h1>
<br><div class="loader"><img src="image/tm.jpg" alt="#" /></div>
A LED display is a flat panel display that uses an array of light-emitting diodes as pixels for a video display
<br>Material used are:

   - 1	Arduino Uno R3
   - 1	220 Ω Resistor
   - 1	LCD 16 x 2
<h1 style="font-size:1vw"><span style="color:black">Code</span></h1>
/*
  LiquidCrystal Library - Hello Gladiators

 This sketch prints "Hello World!" to the LCD
 and shows the time.

  The circuit:
 * LCD RS pin to digital pin 12
 * LCD Enable pin to digital pin 11
 * LCD D4 pin to digital pin 5
 * LCD D5 pin to digital pin 4
 * LCD D6 pin to digital pin 3
 * LCD D7 pin to digital pin 2
 * LCD R/W pin to ground
 * LCD VSS pin to ground
 * LCD VCC pin to 5V
 * 10K resistor:
 * ends to +5V and ground
 * wiper to LCD VO pin (pin 3)

        #include <LiquidCrystal.h>

        LiquidCrystal lcd(12, 11, 5, 4, 3, 2);

        void setup() {
    
        lcd.begin(16, 2);
        lcd.print("Hello, Gladiotors!");
        }

        void loop() {
        lcd.setCursor(0, 1);
        lcd.print(millis() / 1000);
        }

        #include <LiquidCrystal.h>
This line includes the LiquidCrystal library, which provides functions for controlling character LCD modules.

        LiquidCrystal lcd(12, 11, 5, 4, 3, 2);
<br>Declares a LiquidCrystal object named lcd and initializes it with the pins connected to the LCD module. 
<br>The numbers 12, 11, 5, 4, 3, 2 represent the Arduino digital pins connected to the RS, Enable, D4, D5, D6, and D7 pins of the LCD module, respectively.

        void setup() {
        lcd.begin(16, 2);
        lcd.print("Hello, Gladiators!");
        }
<br>The setup() function is a standard Arduino function that is called once when the microcontroller starts.
<br>In this code, the begin() function is called on the lcd object to initialize the LCD module.
<br>The parameters 16 and 2 specify the number of columns and rows of the LCD module, respectively.
<br>The print() function is used to display the string "Hello, Gladiators!" on the LCD module. 
<br>This string will be displayed on the first row of the LCD module.

        void loop() {
        lcd.setCursor(0, 1);
        lcd.print(millis() / 1000);
        }
<br>The loop() function is a standard Arduino function that runs repeatedly after the setup() function.
<br>In this code, the setCursor() function is used to set the cursor position on the LCD module. 
<br>The parameters 0 and 1 specify the column and row position, respectively. This sets the cursor to the first column of the second row.
<br>The print() function is used to display the value of millis() / 1000 on the LCD module. millis() returns the number of milliseconds since the microcontroller started running, and dividing it by 1000 converts it to seconds. This value will be displayed on the second row of the LCD module.

<h1 style="font-size:1.2vw"><span style="color:black">Reference</span></h1>

- [Arduino.cc](https://www.arduino.cc/)
- [Arunino Create](https://create.arduino.cc/editor)
- [Mignrating from Older Version to Newer Version](https://forum.arduino.cc/t/migrating-ide-1-8-19-to-ide-2-0-0/1031923)
- [https://docs.arduino.cc/hardware/uno-rev3](https://docs.arduino.cc/hardware/uno-rev3)
- [Javatpoints](https://www.javatpoint.com/arduino)

<br>
<br><div class="loader"><img src="image/3.jpg" alt="#" /></div>
<br>

For detail Explanation: [Click Here](https://www.w3cschool.cn/arduino/arduino_overview.html)

For a set of example programs of Input and Output: [Click Here](https://www.nexmaker.com/doc/5arduino/Arduino_Input.html) or [Here](https://www.nexmaker.com/doc/5arduino/Arduino_output.html) respectively.
