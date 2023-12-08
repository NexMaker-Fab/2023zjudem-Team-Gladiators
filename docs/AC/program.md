` `**Project one:**

**Simple Shooting game**

This simple game code is implemented in the Processing programming environment. The game involves a player controlled by arrow keys, three enemy drones that move horizontally, and bullets fired by both the player and the drones. The goal is to shoot down the drones while avoiding their bullets.

This code uses the Processing language to create a game window, handle player input, and update the game state. The player can move left and right with the arrow keys and shoot bullets with the spacebar and mousepressed. The drones move horizontally and periodically shoot bullets at the player. The game keeps track of hits and misses for both the player and the drones, and this information is displayed in the console.

Here is the description:

**Game Overview:**

The game features a player-controlled square (representing a player) and three enemy squares (representing drones). The player's objective is to avoid being hit by drones while shooting bullets to eliminate them.

**Controls:**

Player Movement: The player can be moved horizontally using the left and right arrow keys.

Player Shooting: Bullets can be fired by pressing the spacebar or the 's' key.

**Gameplay:**

**Player:** The player is a blue square located at the bottom of the screen. The player can move left and right to avoid collisions with enemy drones.

**Drones:** There are three green squares representing enemy drones. These drones move horizontally across the screen. If a drone collides with the player, it results in a hit, and the player's position is reset.

**Player Bullets:** The player can shoot red bullets upwards to eliminate drones. If a bullet hits a drone, the drone is temporarily disabled and falls down before resetting its position.

Scoring:

**Hits:** When the player successfully eliminates a drone, the hit counter for that drone increases.

**Misses:** If a bullet fired by the player misses a drone and goes off-screen, or if a drone collides with the player, the miss counter increases.

**Drone Behavior:**

Drones periodically shoot bullets towards the player.

When a drone is hit by a player's bullet, it falls down temporarily before resetting its position.

**Game State:**

The game displays counters for player hits and misses, as well as individual hit and miss counters for each drone.

**Technical Details:**

The game is implemented using the Processing programming language.

Object-oriented programming principles are used, with classes for bullets and collision detection functions.

The game features continuous movement of drones, periodic shooting, and bullet animations.


    float playerX, playerY;

    int playerHits = 0;

    int playerMisses = 0;

    int[] droneMisses = {0, 0, 0};

    int droneHits1 = 0;

    int droneHits2 = 0;

    int droneHits3 = 0;

    ArrayList<Bullet> playerBullets = new ArrayList<>();

    ArrayList<Bullet> droneBullets = new ArrayList<>();

    float[] droneX = new float[3];

    float[] droneY = new float[3];

    float droneSpeed = 4; 

    boolean[] droneDirectionRight = {true, true, true};

    boolean[] droneHit = {false, false, false};

    int[] droneHitCounter = {0, 0, 0};

    void setup() {

    `  `size(400, 400);

    `  `playerX = width / 2;

    `  `playerY = height - 30;

    `  `for (int i = 0; i < 3; i++) {

    `    `droneX[i] = random(width - 20);

    `    `droneY[i] = random(height / 4, height / 2);

    `  `}

    }

    void draw() {

    `  `background(220);

    `  `fill(0, 0, 255);

    `  `rect(playerX, playerY, 20, 20);

    `  `fill(0, 255, 0);

    `  `for (int i = 0; i < 3; i++) {

    `    `rect(droneX[i], droneY[i], 20, 20);

    `    `if (hit(playerX, playerY, 20, 20, droneX[i], droneY[i])) {

    `      `playerX = width / 2;

    `      `playerY = height - 30;

    `      `playerHits++;  

    `    `}

    `    `if (frameCount % 60 == 0) {

    `      `float dx = playerX - droneX[i];

    `      `float dy = playerY - droneY[i];

    `      `float angle = atan2(dy, dx);

    `      `droneBullets.add(new Bullet(droneX[i], droneY[i], angle));

    `    `}

    `  `}



    `  `for (int i = droneBullets.size() - 1; i >= 0; i--) {

    `    `Bullet bullet = droneBullets.get(i);

    `    `bullet.update();

    `    `bullet.display();

    `    `if (hit(playerX, playerY, 20, 20, bullet.x, bullet.y)) {

    `      `droneBullets.remove(i);

    `      `playerMisses++;

    `      `updateCounters();

    `    `}

    `    `if (bullet.y > height) {

    `      `droneBullets.remove(i);

    `      `droneMisses[i]++;

    `      `updateCounters();

    `    `}

    `  `}

    `  `fill(255, 0, 0);

    `  `for (int i = playerBullets.size() - 1; i >= 0; i--) {

    `    `Bullet bullet = playerBullets.get(i);

    `    `bullet.update();

    `    `bullet.display();

    `    `for (int j = 0; j < 3; j++) {

    `      `if (hit(droneX[j], droneY[j], 20, 20, bullet.x, bullet.y)) {

    `        `playerBullets.remove(i);

    `        `droneHit[j] = true;

    `        `if (j == 0) {

    `          `droneHits1++;

    `        `} else if (j == 1) {

    `          `droneHits2++;

    `        `} else if (j == 2) {

    `          `droneHits3++;

    `        `}

    `        `updateCounters();

    `      `}

    `    `}

    `    `if (bullet.y < 0) {

    `      `playerBullets.remove(i);

    `      `playerMisses++;

    `      `updateCounters();

    `    `}

    `  `}

    `  `for (int i = 0; i < 3; i++) {

    `    `if (!droneHit[i]) {

    `      `if (droneDirectionRight[i]) {

    `        `droneX[i] += droneSpeed;

    `        `if (droneX[i] > width - 20) {

    `          `droneDirectionRight[i] = false;

    `        `}

    `      `} else {

    `        `droneX[i] -= droneSpeed;

    `        `if (droneX[i] < 0) {

    `          `droneDirectionRight[i] = true;

    `        `}

    `      `}

    `    `} else {



    `      `droneY[i] += 5;

    `      `droneHitCounter[i]++;

    `      `if (droneHitCounter[i] > 30) {

    `        `droneY[i] = random(height / 4, height / 2);

    `        `droneHit[i] = false;

    `        `droneHitCounter[i] = 0;

    `      `}

    `    `}

    `  `}

    `  `if (keyPressed) {

    `    `if (keyCode == LEFT) {

    `      `playerX -= 5;

    `    `} else if (keyCode == RIGHT) {

    `      `playerX += 5;

    `    `}

    `  `}

    `  `playerX = constrain(playerX, 0, width - 20);

    }

    void keyPressed() {

    `  `if (key == ' ') {

    `    `playerBullets.add(new Bullet(playerX + 10, playerY, -PI / 2));

    `  `}

    }

    void updateCounters() {

    `  `println("Player Hits: " + playerHits + " | Player Misses: " + playerMisses);

    `  `for (int i = 0; i < 3; i++) {

    `    `println("Drone " + (i + 1) + " Hits: " + getDroneHits(i) + " | Drone " + (i + 1) + " Misses: " + droneMisses[i]);

    `  `}

    }

    int getDroneHits(int droneIndex) {

    `  `if (droneIndex == 0) {

    `    `return droneHits1;

    `  `} else if (droneIndex == 1) {

    `    `return droneHits2;

    `  `} else if (droneIndex == 2) {

    `    `return droneHits3;

    `  `}

    `  `return 0;

    }

    boolean hit(float rx, float ry, float rw, float rh, float px, float py) {

    `  `return px > rx && px < rx + rw && py > ry && py < ry + rh;

    }

    class Bullet {

    `  `float x, y, speed;

    `  `float angle;

    `  `Bullet(float x, float y, float angle) {

    `    `this.x = x;

    `    `this.y = y;

    `    `this.angle = angle;

    `    `this.speed = 5; 

    `  `}

    `  `void update() {

    `    `x += cos(angle) \* speed;

    `    `y += sin(angle) \* speed;

    `  `}

    `  `void display() {

    `    `ellipse(x, y, 5, 5);

    `  `}

    }

<video width=100% controls><source src="image/prv2.mp4" type="video/mp4">

[Review](https://electronstudio.github.io/pygame-zero-book/chapters/shooter.html)

**Project Two:**

**Graphical User Interface to Controll LED**

To create a Graphic User Interface (GUI) using Processing and Arduino or other microcontrollers, you'll need to combine the design and programming aspects.

**Design the GUI:**

Determine the layout and components you want in your GUI, such as buttons, sliders, text fields, etc.

Sketch out the visual design of your GUI on paper or using design software.

Decide on the overall look and feel, including colors, fonts, and images.

**Set up the hardware:**

Connect your Arduino or other microcontroller to your computer.

Install the necessary drivers and libraries for your microcontroller.

**Write the Arduino code:**

Use the Arduino IDE or another compatible development environment to write the code that will run on the microcontroller.

Define the input/output pins for the components you'll be using in your GUI.

Implement the necessary functionality to read and respond to user input from the GUI.

**Write the Processing code:**

Use the Processing IDE to write the code for the GUI.

Import any necessary libraries for GUI components or communication with the microcontroller.

Define the layout and appearance of the GUI components based on your design.

Implement the logic to send and receive data between the Processing sketch and the microcontroller.

**Test and debug:**

Upload the Arduino code to the microcontroller.

Run the Processing sketch and interact with the GUI to test its functionality.

Debug any issues that arise, such as incorrect data transmission or unresponsive components.

**Refine and iterate:**

Make adjustments to the design and functionality as needed based on testing and feedback.

Continue to refine and iterate on your code and design until you achieve the desired GUI experience.

**Processing part**

The sketch serves as a user interface for controlling external hardware by sending specific commands through a serial port. The graphical buttons and images enhance user interaction, allowing them to toggle LEDs and control a servo motor with a mouse click.

    import processing.serial.\*;
    
    Serial port;
    
    PImage led1OnImage, led1OffImage, led2OnImage, led2OffImage, led3OnImage, led3OffImage, servoOnImage, servoOffImage;

    void setup() {

    `  `size(480, 440);

    `  `led1OnImage = loadImage("image\\light.png");

    `  `led1OffImage = loadImage("image\\light.png");

    `  `led2OnImage = loadImage("image\\light2.png");

    `  `led2OffImage = loadImage("image\\light2.png");

    `  `led3OnImage = loadImage("image\\light3.png");

    `  `led3OffImage = loadImage("image\\light3.png");

    `  `servoOnImage = loadImage("image\\servo.png");

    `  `servoOffImage = loadImage("D:\\desktop\\servo.png");

    `  `led1OnImage = resizeImage(led1OnImage, 360, 120);

    `  `led1OffImage = resizeImage(led1OffImage, 360, 120);

    `  `led2OnImage = resizeImage(led2OnImage, 360, 120);

    `  `led2OffImage = resizeImage(led2OffImage, 360, 120);

    `  `led3OnImage = resizeImage(led3OnImage, 360, 120);

    `  `led3OffImage = resizeImage(led3OffImage, 360, 120);

    `  `servoOnImage = resizeImage(servoOnImage, 360, 120);

    `  `servoOffImage = resizeImage(servoOffImage, 360, 120);

    `  `String[] portList = Serial.list();

    `  `if (portList.length > 0) {

    `    `String portName = portList[0];

    `    `port = new Serial(this, portName, 9600);

    `  `} else {

    `    `println("No serial port available.");

    `  `}

    }

    void draw() {

    `  `background(50);

    `  `drawLeftButtons();

    `  `drawRightButtons();

    }

    void drawLeftButtons() {

    `  `drawButton("LED1 on", 40, 60, led1OnImage);

    `  `drawButton("LED2 on", 40, 160, led2OnImage);

    `  `drawButton("LED3 on", 40, 260, led3OnImage);

    `  `drawButton("SERVO Set", 40, 360, servoOnImage);

    }

    void drawRightButtons() {

    `  `drawButton("LED1 off", 260, 60, led1OffImage);

    `  `drawButton("LED2 off", 260, 160, led2OffImage);

    `  `drawButton("LED3 off", 260, 260, led3OffImage);

    `  `drawButton("SERVO Reset", 260, 360, servoOffImage);

    }

    void drawButton(String label, float x, float y, PImage image) {

    `  `fill(0,0,255);

    `  `textAlign(CENTER, CENTER);


    `  `image(image, x, y);


    `  `text(label, x + image.width / 2, y + image.height / 2);

    }

    void mousePressed() {

    `  `float mx = mouseX;

    `  `float my = mouseY;

    `  `if (isMouseOverButton(mx, my, 40, 260, led3OnImage.width, led3OnImage.height)) {

    `    `port.write('3');

    `    `delay(200); 

    `  `} else if (isMouseOverButton(mx, my, 260, 260, led3OffImage.width, led3OffImage.height)) {

    `    `port.write('7');

    `    `delay(200); 

    `  `} else {

    `    `handleButtonClicks(mx, my);

    `  `}

    }


    void handleButtonClicks(float mx, float my) {

    `  `if (isMouseOverButton(mx, my, 40, 60, led1OnImage.width, led1OnImage.height)) {

    `    `port.write('1');

    `  `} else if (isMouseOverButton(mx, my, 40, 160, led2OnImage.width, led2OnImage.height)) {

    `    `port.write('2');

    `  `} else if (isMouseOverButton(mx, my, 40, 360, servoOnImage.width, servoOnImage.height)) {

    `    `port.write('4');

    `  `} else if (isMouseOverButton(mx, my, 260, 60, led1OffImage.width, led1OffImage.height)) {

    `    `port.write('5');

    `  `} else if (isMouseOverButton(mx, my, 260, 160, led2OffImage.width, led2OffImage.height)) {

    `    `port.write('6');

    `  `} else if (isMouseOverButton(mx, my, 260, 360, servoOffImage.width, servoOffImage.height)) {

    `    `port.write('8');

    `  `}

    }

    boolean isMouseOverButton(float mx, float my, float x, float y, float width, float height) {

    `  `return mx > x && mx < x + width && my > y && my < y + height;

    }

    PImage resizeImage(PImage original, int targetWidth, int targetHeight) {

    `  `float aspectRatio = (float) original.width / original.height;

    `  `float targetRatio = (float) targetWidth / targetHeight;

    `  `int newWidth, newHeight;

    `  `if (aspectRatio > targetRatio) {

    `    `newWidth = targetWidth;

    `    `newHeight = (int) (targetWidth / aspectRatio);

    `  `} else {

    `    `newWidth = (int) (targetHeight \* aspectRatio);

    `    `newHeight = targetHeight;

    `  `}

    `  `PImage resizedImage = createImage(newWidth, newHeight, ARGB);

    `  `resizedImage.copy(original, 0, 0, original.width, original.height, 0, 0, newWidth, newHeight);

    `  `return resizedImage;

    }



**Arduino part:**

    #include <Servo.h>

    Servo servoMotor;

    int led1Pin = 10;

    int led2Pin = 11;

    int led3Pin = 12;

    int servoPin = 9;

    void setup() {

    `  `pinMode(led1Pin, OUTPUT);

    `  `pinMode(led2Pin, OUTPUT);

    `  `pinMode(led3Pin, OUTPUT);

    `  `servoMotor.attach(servoPin);  // Attaches the servo to the specified pin

    `  `Serial.begin(9600);

    }

    void loop() {

    `  `if (Serial.available() > 0) {

    `    `char command = Serial.read();

    `    `switch (command) {

    `      `case '1':

    `        `digitalWrite(led1Pin, HIGH);

    `        `break;

    `      `case '2':

    `        `digitalWrite(led2Pin, HIGH);

    `        `break;

    `      `case '3':

    `        `digitalWrite(led3Pin, HIGH);

    `        `break;

    `      `case '4':

    `        `servoMotor.write(720);  // Rotate the servo to 90 degrees

    `        `break;

    `      `case '5':

    `        `digitalWrite(led1Pin, LOW);

    `        `break;

    `      `case '6':

    `        `digitalWrite(led2Pin, LOW);

    `        `break;

    `      `case '7':

    `        `digitalWrite(led3Pin, LOW);

    `        `break;

    `      `case '8':

    `        `servoMotor.write(0);  // Rotate the servo to 0 degrees

    `        `break;

    `      `default:

    `        `break;

    `    `}

    `  `}

    }

The above Programming can not display the required result one without the other. Because they are dependent on each other. Without the use of an external device like a laptop, direct integration between Processing and Tinkercad has not been possible yet.  

**Processing part Image**

<img style="float: center;" width=100% src="image/prar.jpg">

**Arduino Part** ( when we run it in the Tinkercad, nothing is displayed.)

<img style="float: center;" width=100% src="image/arpr.jpg">

**Final Result of the Processing and Arduino.**

<video width=100% controls><source src="image/pra.mp4" type="video/mp4">

[Review](https://www.hackster.io/hardikrathod/control-arduino-using-gui-arduino-processing-2c9c6c)
