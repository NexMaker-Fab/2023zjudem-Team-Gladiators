### WiFi-Controlled Light, Door, and Fan for People with Mobility Disability Using Web Interface Control
#### Introduction
This project aims to develop WiFi-controlled solutions for lights, doors, and fans specifically designed to address the unique needs of disabled individuals. By leveraging WiFi technology and incorporating accessibility features, we provided innovative solutions that enhance independence, convenience, and comfort for disabled individuals.
### Literature Review
Before we started doing our final project,we have tried to conduct thorough researchs on recently published articles, forums and websites. Here are some of the websites which are relevant to our project.
#### The integration of smart home technology:
The integration of smart home technology has been a game-changer for individuals with disabilities, particularly those with mobility challenges. The ability to control various aspects of one's environment through a web interface can significantly enhance independence and quality of life. This report synthesizes key points from recent sources to explore the benefits and considerations of using WiFi-controlled lights, doors, and fans for individuals with mobility disabilities.

#### Accessibility and the ADA:
The Americans with Disabilities Act (ADA) emphasizes the importance of accessible web content for people with disabilities. Inaccessible web features can prevent equal access to information and services . The ADA applies to public entities and businesses, which have the flexibility to choose how to make their online services accessible. Technical standards such as the Web Content Accessibility Guidelines (WCAG) and Section 508 Standards offer guidance on ensuring web accessibility [(1)](https://www.ada.gov/resources/web-guidance/#:~:text=Inaccessible%20web%20content%20means%20that%20people%20with%20disabilities%20are%20denied%20equal%20access%20to%20information).

#### Smart Home Technology for Disabled Individuals:
Smart home devices have revolutionized living spaces, enhancing convenience and quality of life for disabled individuals. These technologies prioritize accessibility and independence, assisting with safety, daily activities, and communication . They can also integrate with healthcare systems for emergencies . A central control hub, typically an app or voice assistant, allows for remote management of smart devices [(2)](https://www.ecovacs.com/us/blog/smart-home-devices-disabled-persons).

#### Enhancing Independence with Smart Home Devices
Smart home technology can empower individuals with disabilities to live more independently by simplifying everyday tasks such as turning on lights, opening doors, or adjusting fans . These devices can provide notifications, remote access control, and hands-free operation through integration with other devices . The setup process is generally straightforward, using a smartphone and an app . Smart home devices not only offer independence but can also lead to energy savings and a more comfortable living environment [(3)](https://www.nytimes.com/wirecutter/reviews/best-assistive-smart-home-technology-for-disabled/).
### What problems are we solving?

According to our review, voice controlled light and door system doesn't secure individual's  **privacy concern and potential disturbance**. Thus, we decided to develop  a project with a **web-based control interface**, providing a discreet and personalized **alternative** to voice controlled system. While voice control is a common method for web navigation and device control, it may not be universally suitable due to privacy considerations or the potential to disrupt others. The proposed web interface control is an ideal solution to addresses these concerns, offering an independence,accessibility and  a customizable solution tailored to the user's individual needs.
### How the project has been done?
#### A: Required Hardwares
<img style="float: center;" width=700 src="image/pro1.jpg">
<img style="float: center;" width=700 src="image/pro2.jpg">
<img style="float: center;" width=700 src="image/pro3.jpg">
<img style="float: center;" width=700 src="image/pro4.jpg">
<img style="float: center;" width=700 src="image/pro5.jpg">
<img style="float: center;" width=700 src="image/pro6.jpg">
<img style="float: center;" width=700 src="image/pro7.jpg">
<img style="float: center;" width=700 src="image/pro8.jpg">
<img style="float: center;" width=700 src="image/pro9.jpg">
<img style="float: center;" width=700 src="image/pro10.jpg">
<img style="float: center;" width=700 src="image/pro11.jpg">
<img style="float: center;" width=700 src="image/pro12.jpg">

#### B: Software Required:
[IDE](https://www.arduino.cc/en/software)
<br>
<br>
[LaserCAD v8.13.7](https://www.joystarlaser.com/m/index.php?a=lists&catid=15)
<br><br>
<img style="float: center;" width=700 src="image/pro43.png">
<img style="float: center;" width=700 src="image/pro44.png">
<img style="float: center;" width=700 src="image/pro45.png">
<img style="float: center;" width=700 src="image/pro46.png">

[Fusion 360](https://www.autodesk.com/productsfusion-360/overview)

The house shown below is designed and assembled on Fusion 360.
<br><div><br><video width=100% height=56.25% controls><source src="image/pro23.mp4" type="video/mp4">
</video></div>

**Design History**
<br><div><br><video width=100% height=56.25% controls><source src="image/pro24.mp4" type="video/mp4">
</video></div>
Section view and 2D drawing views with detail dimension
<img style="float: center;" width=700 src="image/pro25.jpg">
<br>

**Lamp**

<img style="float: center;" width=700 src="image/pro36.png">
<img style="float: center;" width=700 src="image/pro37.png">
<img style="float: center;" width=700 src="image/pro38.png">
<img style="float: center;" width=700 src="image/pro39.png">
<img style="float: center;" width=700 src="image/pro40.png">
<img style="float: center;" width=700 src="image/pro41.png">
<img style="float: center;" width=700 src="image/pro42.png">

[3D printer](https://www.flashforge.com/product-detail/FlashPrint-slicer-for-flashforge-fdm-3d-printers)

The house designed on fusion 360 is printed using a Flash Forge Guider IIs printer to demonstrate the opening and closing doors automatically using Arduino.
<br><br>
<img style="float: center;" width=700 src="image/pro26.jpg">

#### C: Programming Used
**C++**

C++ is used as the programming language for the microcontroller firmware. The C++ code controls the ESP8266 module, handles HTTP requests, and interacts with the hardware components such as the servo motor, LED, and fan. It sets up the web server, defines request handlers, and performs the desired actions based on the incoming requests. C++ is commonly used for low-level programming tasks and is well-suited for embedded systems.

**HTML**:

HTML (Hypertext Markup Language) is used for creating the web page that allows users to interact with the microcontroller. In the code, HTML is embedded within the C++ code as strings. The HTML code defines the structure, layout, and content of the web page. It includes buttons to control the LED, servo motor (door), and fan. When a user interacts with the buttons, HTTP requests are sent to the microcontroller to perform the requested actions.

**JAVASCRIPT**

JavaScript is used to add interactivity to the web page. In the code, JavaScript code is embedded within the HTML code as inline scripts. JavaScript is responsible for handling button clicks and sending HTTP requests to the microcontroller. When a user clicks a button, the JavaScript code triggers an HTTP request with the appropriate command to control the microcontroller. It enables the web page to dynamically update and communicate with the microcontroller in real-time.

In summary, C++ is used for the microcontroller firmware and handling HTTP requests, HTML is used for creating the web page structure and content, and JavaScript is used for adding interactivity to the web page and sending HTTP requests to control the microcontroller.
## How this project has been done?
**1. Working Principle of Light Bulb:**
<br> <br> In this WiFi-controlled system, a high-power Light is utilized as a controllable light source. This Light, physically larger than standard indicator LEDs, is connected to pin D3 on an ESP8266 microcontroller. The ESP8266, equipped with WiFi capabilities, hosts a web server that allows users to control the connected light through a user-friendly web interface.

**Code Integration:**
<br>

**Physical Setup:**

The high-power light is connected to pin D3 (const int ledPin = D3;) on the ESP8266.
<br>
<br>
<img style="float: center;" width=auto src="image/pro33.jpg">

**Web Interface:**

The web interface is accessible through the root endpoint (/). Users can interact with the interface to control various functions, including the high-power LED.

**Light Control in Web Interface:**

Within the web interface, there are buttons designed to control the high-power LED. The buttons are styled with background colors and icons for a visually appealing user experience.

<img style="float: center;" width=auto src="image/pro13.jpg">
<img style="float: center;" width=auto src="image/pro19.jpg">

**Handling Light Commands:**

The server's handleCommand function processes incoming POST requests, including those for controlling the LED. When a command such as 'turn-on-led' or 'turn-off-led' is received, it triggers the corresponding action in the code.

  <img style="float: center;" width=auto src="image/pro16.jpg">
 <br><div><br><video width=100% height=56.25% controls><source src="image/pro27.mp4" type="video/mp4">
</video></div>

**Summary:**

The system integrates a high-power LED as a controllable light source within a WiFi-controlled environment. Users can access a web interface served by the ESP8266 to turn the LED on and off, providing a convenient and remote means of controlling the lighting in their application. This demonstrates the versatility of the ESP8266 microcontroller for creating IoT (Internet of Things) projects with web-based interfaces.

**2. Working Principle of the Door System:**
<br><br>
In this WiFi-controlled system, a physical door is integrated, and its movement is controlled through the web interface. The door system involves a servo motor connected to pin D5 on the ESP8266 microcontroller, allowing users to remotely open and close the door through a user-friendly web interface.

**Code Integration:**

**Physical Setup:**
<br><br>
A real door is connected to a servo motor, which is connected to pin D5 (const int servoPin = D5;) on the ESP8266. The servo motor is responsible for physically moving the door.
<br><br>
<img style="float: center;" width=auto src="image/pro34.jpg">
**Web Interface:**

The web interface, accessible through the root endpoint (/), provides buttons for controlling the door's movement.
html

<img style="float: center;" width=auto src="image/pro14.jpg">
<img style="float: center;" width=auto src="image/pro20.jpg">

**Handling Door Commands:**

The server's handleCommand function processes incoming POST requests, including those for controlling the door. When a command such as 'open-door' or 'close-door' is received, it triggers the corresponding action in the code.

<img style="float: center;" width=auto src="image/pro17.jpg">
<br><div><br><video width=100% height=56.25% controls><source src="image/pro28.mp4" type="video/mp4">
</video></div>

**Summary:**

The door control system in this WiFi-controlled environment allows users to remotely open and close a physical door through the web interface. The integration of a servo motor and the corresponding code functions demonstrate how the ESP8266 microcontroller can be used to control real-world devices, making it suitable for home automation or access control applications. This adds a practical dimension to the IoT project, allowing users to interact with and control physical elements within their environment over the internet.

**3. Working Principle of the Fan:**

In this WiFi-controlled system, a physical fan is integrated, and its operation is controlled through the web interface. The fan system involves a relay or transistor connected to pin D8 on the ESP8266 microcontroller, allowing users to remotely turn the fan on and off through a user-friendly web interface.

**Code Integration:**

**Physical Setup:**

A real fan is connected to a relay or transistor, which, in turn, is connected to pin D8 (const int fanPin = D8;) on the ESP8266. The relay or transistor is responsible for controlling the electrical power to the fan, enabling remote control.
<br><br>
<img style="float: center;" width=auto src="image/pro31.jpg">

**Web Interface:**

The web interface, accessible through the root endpoint (/), provides buttons for controlling the fan's operation.

<img style="float: center;" width=auto src="image/pro15.jpg">
<img style="float: center;" width=auto src="image/pro21.jpg">

**Handling Fan Commands:**

The server's handleCommand function processes incoming POST requests, including those for controlling the fan. When a command such as 'turn-on-fan' or 'turn-off-fan' is received, it triggers the corresponding action in the code.

<img style="float: center;" width=700 src="image/pro18.jpg">
<br><div><br><video width=100% height=56.25% controls><source src="image/pro29.mp4" type="video/mp4">
</video></div>

**Summary:**

The fan control system in this WiFi-controlled environment allows users to remotely turn a physical fan on and off through the web interface. The integration of a relay or transistor and the corresponding code functions demonstrate how the ESP8266 microcontroller can be used to control real-world devices, making it suitable for home automation or climate control applications. This adds practical functionality to the IoT project, enabling users to interact with and control physical elements within their environment over the internet.

**The Overall Physical and Web Interface Description**

In this WiFi-controlled system, the ESP8266 microcontroller facilitates remote control over real-world devices. The system includes a high-power LED on pin D3, a physical door controlled by a servo motor on pin D5, and a real fan controlled by a relay or transistor on pin D8. Through a user-friendly web interface hosted on the ESP8266, users can turn the LED on/off, open/close the door, and turn the fan on/off, showcasing the versatility of the microcontroller in managing diverse physical elements within an IoT framework.

**The Physical Setup:**

<img style="float: center;" width=auto src="image/pro32.jpg">

**Web Interface:**

<img style="float: center;" width=auto src="image/pro22.jpg">
<br><div><br><video width=100% height=56.25% controls><source src="image/pro30.mp4" type="video/mp4">
</video></div>

## Innovation
WiFi-enabled solutions for lights, doors, and fans are poised to revolutionize the way we interact with our surroundings. These cutting-edge technologies boast innovative features meticulously crafted to enhance accessibility, offering a seamless experience for individuals with diverse needs. Tailored customization settings provide users with unprecedented control over their environment, allowing them to personalize their surroundings according to their preferences.
Moreover, these advancements prioritize privacy concerns, ensuring that users have the peace of mind that their data is handled securely. Recognizing the importance of minimizing potential disturbances, these solutions are designed to operate discreetly, providing a harmonious and unintrusive experience.
With a focus on inclusivity, these smart home technologies are specifically engineered to cater to the unique requirements of disabled individuals, fostering a more inclusive and accommodating living environment. By seamlessly integrating technology and thoughtful design, WiFi-controlled systems for lights, doors, and fans are at the forefront of creating homes that are not only smart but also considerate of the diverse needs of their inhabitants. 
The development of a web interface control for WiFi-connected lights, doors, and fans has successfully addressed  **customization**,  **privacy concerns** and **potential disturbances**. This innovative solution offers discreet control options, personalized settings, and the ability to manage devices remotely.

#### 1: Customizable setting:
The WiFi-controlled devices will offer customizable settings, allowing users to personalize lighting levels, fan speeds, and door operation to meet their specific needs. This flexibility ensures that disabled individuals can create a comfortable living environment tailored to their preferences. 

#### 2. Discreet Control:
 A web interface allows individuals to control their devices without the need for vocal interaction, providing a more discreet control method. This can be particularly beneficial for individuals who value their privacy and prefer not to have audible commands that may be overheard by others nearby. Therefore, The web interface provides a discreet method of controlling devices, eliminating the need for vocal commands that may disturb others or compromise privacy.
#### 3: Personalization and privacy settings:
Users can customize the web interface according to their preferences, such as adjusting font sizes, choosing high contrast options, or enabling privacy settings. This enhances user comfort and privacy during device control.
#### 4: Remote management:
With the web interface, individuals can conveniently manage their WiFi-connected devices from a distance. This eliminates the need for physical proximity, ensuring privacy and reducing disturbances caused by others accessing the devices.
#### 5: Eliminated Disturbances:
By using a web interface, individuals can control their devices without causing potential disturbances to others in the vicinity. Unlike voice control, which may require audible commands, a web interface allows for silent control, minimizing disruptions to others who may be sharing the same space.
#### 6: Pivacy and Security Measures:
The development of the web interface includes robust privacy and security measures. These measures ensure encryption protocols, secure authentication methods, and data protection mechanisms are in place to safeguard user privacy and prevent unauthorized access to the devices.
### Market Analysis for WiFi-Controlled Lighting, Door, and Fan Systems
The assistive technology market is expanding rapidly, with a significant portion of this growth attributed to smart home solutions that cater to the needs of disabled individuals. The integration of WiFi-controlled systems for lighting, doors, and fans is a prime example of how technology is being adapted to improve the quality of life for this demographic.
#### 1: Projected Market Growth:
The global assistive technology market is expected to reach a value of $27.9 billion by 2024, growing at a compound annual growth rate (CAGR) of 7.8% [(1)](https://www.va.gov/housing-assistance/disability-housing-grants/#:~:text=Changing%20a%20home%20might%20involve%20installing%20ramps%20or%20widening%20doorways). This growth is indicative of the increasing demand for assistive devices and smart home solutions that offer greater independence and improved living conditions for people with disabilities.
#### 2: Opportunities for WiFi-Controlled Solutions
The projected market growth presents a significant opportunity for the development and implementation of WiFi-controlled light, door, and fan solutions. These systems are designed to provide users with disabilities the ability to easily manage their environment, contributing to a more accessible and convenient home setting[(2)](https://www.va.gov/housing-assistance/disability-housing-grants/#:~:text=Disability%20housing%20grants%20for%20Veterans).
#### 1: Projected Market Growth:
The global assistive technology market is expected to reach a value of $27.9 billion by 2024, growing at a compound annual growth rate (CAGR) of 7.8% [(1)](https://www.va.gov/housing-assistance/disability-housing-grants/#:~:text=Changing%20a%20home%20might%20involve%20installing%20ramps%20or%20widening%20doorways). This growth is indicative of the increasing demand for assistive devices and smart home solutions that offer greater independence and improved living conditions for people with disabilities.
#### 2: Opportunities for WiFi-Controlled Solutions
The projected market growth presents a significant opportunity for the development and implementation of WiFi-controlled light, door, and fan solutions. These systems are designed to provide users with disabilities the ability to easily manage their environment, contributing to a more accessible and convenient home setting[(2)](https://www.va.gov/housing-assistance/disability-housing-grants/#:~:text=Disability%20housing%20grants%20for%20Veterans).
### Key Technology Analysis and Potential Tech Problems
To develop WiFi-controlled devices for disabled individuals, we will leverage key technologies such as WiFi connectivity, voice recognition, and user-friendly interfaces. These technologies have already demonstrated their efficacy and reliability in the market.

However, it is crucial to address potential tech problems that may arise during the development and implementation process. These problems may include connectivity issues, compatibility challenges with different voice assistants, and ensuring robust security measures. Rigorous testing and quality control processes will be implemented to mitigate these risks and ensure the devices meet the highest standards.

### Materials and Manufacturing
In line with sustainable development goals, we will prioritize the use of environmentally friendly materials and sustainable manufacturing practices. This includes sourcing materials from suppliers with responsible sourcing policies, minimizing waste during the manufacturing process, and optimizing energy consumption in production facilities. By adopting sustainable practices, we can contribute to reducing emissions and waste, as well as promoting resource efficiency.

### Solving Sustainable Development Goals (SDGs)
The proposed WiFi-controlled solutions for disabled individuals align with several SDGs, including:

#### Goal 3:
By enhancing independence and accessibility, our solutions promote the well-being and quality of life for disabled individuals.

#### Goal 10: 
WiFi-controlled devices designed for disabled individuals address the unique challenges they face, reducing inequalities and promoting inclusivity.

#### Goal 11:
Our solutions contribute to the development of smart and accessible cities, fostering sustainable communities that cater to the needs of all individuals.

### Conclusion
The proposed WiFi-controlled solutions for lights, doors, and fans aim to address the specific needs of disabled individuals, promoting independence, accessibility, and safety. By leveraging WiFi technology, incorporating innovative features, and aligning with the SDGs, we can create products that make a positive impact on the lives of disabled individuals and contribute to a more inclusive and sustainable future.
