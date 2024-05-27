<h1 style="color: #e19cab;">Processing</h1>

<font size="5"><h2 style="color: #e19cab;">1. Learn Processing</h2></font>
<h3 style="color: #e19cab;"> What is Processing</h3>

- Processing is an open-source programming language specifically designed for visual artists, designers, researchers, and beginners. The primary goal of this language is to provide a more accessible way to learn the fundamentals of computer programming, especially the comprehension of objects in a visual context.

- The Processing language is based on Java, but its design is simple, making it easier for beginners to use. With Processing, you can create static, dynamic, or interactive pieces of artwork. It has extensive applications in many fields, including image processing, animation, and interactive design.

- Processing provides users with a rich set of graphic and interactive libraries, and it can also interact with hardware conveniently. Therefore, it is widely welcomed in the fields of makers, electronic art, data visualization, and so on.

<h3 style="color: #e19cab;"> How to Download</h3>

1. Open the official Processing website: https://processing.org/

2. On the homepage of the website, click the "Download" button in the top right corner.

3. You will see versions for several operating systems, including Windows, Mac OS, and Linux. Choose the appropriate version based on your computer's operating system.

4. After the download is complete, unzip the file then run the Processing application to install it.

5. Once installed successfully, you can start using the Processing programming language.

Please note: Make sure your computer meets the system requirements for Processing. If you encounter any problems during the installation, you can refer to the FAQ on the official website or seek help from the online community.

<h3 style="color: #e19cab;"> Language</h3>

- Processing is a programming language based on Java, designed for visual programming. 

- Here is a basic sketch example: 

```java
/**
 * Setup and Draw. 
 * The code in setup() is run once when the program starts.
 * The code inside the draw() function runs continuously from top to bottom until the program is stopped. The
 * Reference from https://processing.org/examples/setupdraw.html

 **/
void setup() {
size(800, 600);
background(102);
}

void draw() {
stroke(255);
if (mousePressed) {
line(mouseX, mouseY, pmouseX, pmouseY);
}
}
```

- Simply put, a Processing program is primarily built with two functions: `setup()` and `draw()`. The `setup()` function is mainly used for some settings that need to be performed only once when the program starts. The `draw()` function is continuously and repeatedly called during the operation of your program, handling all animations and real-time updates.

- Moreover, Processing includes a large number of user-friendly functions to implement complex visual effects, such as shapes, colors, images, pixels, text, 3D effects, and more.

<h3 style="color: #e19cab;"> Shape</h3>

Processing provides a range of functions that allow you to easily draw various shapes. These include:

1. `point()`: Draws a point.
2. `line()`: Draws a line.
3. `rect()`: Draws a rectangle.
4. `ellipse()`: Draws an ellipse or circle.
5. `triangle()`: Draws a triangle.
6. `quad()`: Draws a quadrilateral.
7. `arc()`: Draws an arc.
8. `bezier()`: Draws a Bezier curve.
9. `curve()`: Draws a smooth curve.

Each function has its specific parameters that you need to set according to your specific needs and expected results. You can find the specific usage methods and more shape functions on the official [Processing website](https://processing.org/).

<h3 style="color: #e19cab;"> Shape</h3>
Example：

```java
void setup() {
  size(500, 500);     // Set the canvas size to 500x500 pixels
  background(255);    // Set the background color to white
}

void draw() {
  fill(255, 0, 0);     // Set the fill color to red
  rect(50, 50, 200, 200);     // Draw a rectangle positioned at (50,50) with a width and height of 200

  fill(0, 255, 0);    // Set the fill color to green
  ellipse(350, 250, 100, 150);     // Draw an ellipse centered at (350,250) with a width of 100 and a height of 150

  fill(0, 0, 255);    // Set the fill color to blue
  triangle(100, 300, 250, 450, 50, 450);     // Draw a triangle with vertices at (100,300), (250,450), and (50,450)
}
```

<h3 style="color: #e19cab;"> For reference</h3>

1. [Processing official website](https://processing.org)：Complete reference materials, tutorials, examples, and communities are provided.
2. [OpenProcessing](https://www.openprocessing.org)：A platform for Processing users to create and share great works.
3. [Khan Academy](https://www.khanacademy.org/computing/computer-programming)：There are a series of tutorials on computer programming, including using Processing.js.
4. [动手学 Processing](https://www.bilibili.com/video/BV1zE411u7Vj)：This is a very popular Chinese Processing video tutorial.
5. [Coding Train](https://thecodingtrain.com)：MIT professor Daniel Shiffman's YouTube channel offers many tutorials on animation and visual effects created in Processing.

<font size="5"><h2 style="color: #e19cab;">2. New tools</h2></font>
<h3 style="color: #e19cab;"> Touch designer</h3>

- TouchDesigner is a real-time visual editing software developed by the Canadian company Derivative. It is based on a "node system", each node has its own function, suitable for real-time visual creation and development in music, performance, art and other fields.


><strong>Live action: TouchDesigner allows you to manipulate and control content in real time, which is useful when creating effects, developing apps, or working in the field.</strong>

><strong>Node system: TouchDesigner's design is based on nodes, each of which performs a specific task, such as processing images, transforming data, and so on. In this system, you can control and regulate the data flow between nodes through parameters and Settings.</strong>

><strong>Programming: Although TouchDesigner is a visual tool, it also allows users to complete complex operations and extensions through Python programming.</strong>

><strong>Flexible input/output: TouchDesigner can receive and send information in a variety of ways, including sound, images, video, MIDI, OSC, and DMX.</strong>

><strong>Real-time rendering: TouchDesigner supports high-quality 3D rendering and interaction with major real-time rendering engines such as Unreal Engine and Unity.</strong>

><strong>Community support: TouchDesigner has a very active community, which is a great learning resource for beginners, and many tutorials and engineering references can be found.</strong>

<div><img width="1000" src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/8e0ad8c8d313aab8d0f2c3dfa734c81a679d0070/images/processing/processing.gif"></div>

<h3 style="color: #e19cab;"> For reference</h3>

1. [Processing Official Website](https://processing.org)：They provide complete reference materials, tutorials, examples, and a community.
2. [OpenProcessing](https://www.openprocessing.org)：A platform for Processing users to create and share their work.
3. [Khan Academy](https://www.khanacademy.org/computing/computer-programming)：A series of programming tutorials, including using Processing.js.
4. [Coding Train](https://thecodingtrain.com)：MIT professor Daniel Shiffman's YouTube channel, offering many tutorials on animation and visual effects created in Processing.
5. [动手学 Processing](https://www.bilibili.com/video/BV1zE411u7Vj)：A very popular Chinese Processing video tutorial.

<h3 style="color: #e19cab;"> Unity</h3>

- Unity is a highly popular cross-platform game development engine, extensively used for creating both 2D and 3D games. Additionally, it is utilized for producing interactive content, animations, visual effects, and augmented reality, etc.

><strong>Cross-platform compatibility: Unity supports the development of games and applications that can run on multiple platforms, including Windows, Mac, Linux, Android, iOS, as well as VR/AR devices, etc.</strong>

><strong>Powerful rendering engine: Unity provides a robust rendering engine, supporting detailed environmental and lighting effects, enabling advanced graphic effects and realistic physics simulation.</strong>

><strong>Easy-to-use editor environment: Unity offers a visual editing environment, making it straightforward for scene construction, character modeling, and game physics and logic programming.</strong>

><strong>Component-based workflow: Unity's design utilizes a "component system," meaning that you can add various functionalities to game objects, and control and modify these components through programming or Boolean operations.</strong>

><strong>Programming language: Unity uses C# for programming, a powerful yet relatively easy-to-learn language, suitable for beginners.</strong>

><strong>Rich resources and community: The Unity Asset Store provides a vast array of pre-made content, including models, textures, sound effects, etc. The strong Unity community also offers endless resources and support to developers.</strong>

<div><img width="1000" src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/1cbc16452eb15ca51e5bb83879b2d09d8dc46865/images/processing/UNITY.gif"></div>

<h3 style="color: #e19cab;"> Language</h3>

Example：

```c++
// Import the Unity engine namespace
using UnityEngine;

// Create a public class named RotateObject that inherits from MonoBehaviour
public class RotateObject : MonoBehaviour
{
    // This is a public floating point number that represents the rotation speed, calculated in degrees per second.
    public float speed = 50f;

    // Update is Unity's built-in frame update method, automatically called at every frame render.
    void Update()
    {
        // Using the transform.Rotate method, make the game object rotate around the y-axis (Vector3.up) at a given speed (speed * Time.deltaTime).
        // Time.deltaTime is the fixed frame time, used to ensure that the game runs at the same speed on all hardware.
        transform.Rotate(Vector3.up, speed * Time.deltaTime);
    }
}
```
<h3 style="color: #e19cab;"> For reference</h3>

1. [Unity Official Website](https://unity.com)：They provide complete reference materials, tutorials, examples, and a community.
2. [Unity Learn](https://learn.unity.com)：It contains various Unity learning materials and courses.
3. [Unity Asset Store](https://assetstore.unity.com)：There is a wealth of ready-to-use assets and tools to accelerate your Unity project development.
4. [Unity Documentation](https://docs.unity3d.com/Manual/index.html)：Detailed document explaining Unity features and development workflows.
5. [Brackeys](https://www.youtube.com/user/Brackeys)：The YouTube channel offers many Unity development tutorials. Very suitable for beginners.

<font size="5"><h2 style="color: #e19cab;">3. One Keyboard interaction demo in processing</h2></font>

```java
/**
*Do one demo in processing which can use mouseto interactive
*2024/5/25
*By BUNBUN Team
**/

void setup(){
  size(800,600);    // Set the size of the canvas
  background(255,255,183);    // Set the background color
}

void draw(){
  // Tail
  stroke(183,223,255);    // Set the color of the stroke
  fill(112,160,252);    // Set the color to fill the shape
  triangle(380,40,560,130,480,160);     // Draw tail

  // Head
  fill(171,199,252);    // Set the color to fill the shape
  stroke(183,223,255);    // Set the color of the stroke
  arc(380,100,200,120,PI,TWO_PI);     // Draw part of the head
  arc(480,130,80,70,PI+HALF_PI,TWO_PI+HALF_PI); // Draw part of the head
  arc(280,130,80,70,HALF_PI,PI+HALF_PI);    // Draw part of the head

  // Arms
  fill(112,160,252);    // Set the color to fill the shape
  ellipse(280,210,50,100);    // Draw left arm
  ellipse(480,210,50,100);    // Draw right arm

  // Body
  stroke(171,199,252);    // Set the color of the stroke
  fill(171,199,252);    // Set the color to fill the shape
  rect(280,100,200,65);     // Draw top part of the body
  rect(280,165,200,150);    // Draw bottom part of the body

  // Feet
  fill(112,160,252);    // Set the color to fill the shape
  ellipse(300,320,50,80);     // Draw left foot
  ellipse(460,320,50,80);     // Draw right foot

  // Belly
  fill(255,255,255);    // Set the color to fill the shape
  arc(380,160,200,120,PI,TWO_PI);     // Draw belly

  // Eyes
  fill(0,0,0);    // Set the color to fill the shape
  ellipse(320,100,20,30);     // Draw left eye
  ellipse(420,100,20,30);     // Draw right eye

  // Collar
  stroke(0,0,0);    // Set the color of the stroke
  strokeWeight(4);    // Set the thickness of the stroke
  fill(255,170,196);    // Set the color to fill the shape
  ellipse(370,125,70,40);     // Draw collar

  // Teeth
  fill(255,255,255);    // Set the color to fill the shape
  strokeWeight(3);    // Set the thickness of the stroke
  triangle(340,115,345,125,350,110);    // Draw one tooth
  triangle(355,110,360,120,365,106);     // Draw another tooth
  triangle(370,106,375,118,380,107);    // Draw another tooth
  triangle(385,108,390,120,395,112);    // Draw another tooth

  // Cheeks
  fill(255,183,205);    // Set the color to fill the shape
  strokeWeight(4);    // Set the thickness of the stroke
  ellipse(300,120,20,10);     // Draw left cheek
  ellipse(440,120,20,10);     // Draw right cheek

  // Mouth
  fill(255,255,255);     // Set the color to fill the shape
  stroke(171,199,252);    // Set the color of the stroke
  strokeWeight(0);    // Set the thickness of the stroke
  arc(380,160,175,270,0,PI);    // Draw mouth

  // Animation
  if(mousePressed){     // If the mouse is pressed...
     if(mouseButton==LEFT){     // And if the mouse button clicked is the left one...
      translate(30,40);     // Shift the coordinate system by 30 in the x-axis and 40 in the y-axis
      fill(255);    // Set the color to fill the shape
      ellipse(295, 98, 20, 20);     // Draw an ellipse
      ellipse(260, 97, 20, 20);     // Draw another ellipse
      ellipse(230, 94, 20, 20);     // Draw another ellipse
    } else {
      if(mouseButton==RIGHT){       // And if the mouse button clicked is the right one...
        fill(255, 183, 205);        // Set the color to fill the shape
        strokeWeight(3);            // Set the thickness of the stroke
        stroke(0);                 // Set the color of the stroke
        ellipse(300,120,30,20);   // Draw an ellipse
        ellipse(440,120,30,20);   // Draw another ellipse
        translate(0, 0);  // Reset the coordinate system
        fill(0);          // Set the color to fill the shape
        stroke(0);        // Set the color of the stroke
        scale(1.1);      // Increase the size of the following shapes
        ellipse(290,90,30,30);    // Draw an ellipse
        ellipse(382,90,30,30);    // Draw another ellipse
      }  
    }
  }
}
``` 
<div><img width="1000" src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/36bc1b7b7eef4cc2665ef1275194eca45d82a2f7/images/processing/processing%20%E4%BD%9C%E4%B8%9A2%E9%BC%A0%E6%A0%87%E4%BA%A4%E4%BA%92.gif"></div>

<font size="5"><h2 style="color: #e19cab;">4. One demo in processing and arduino</h2></font>

<div><img width="1000" src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/9bae5b5ebc2bb9b7ca75c4bb8f0c4472ceb0f42c/images/processing/arduino%E8%B6%85%E5%A3%B0%E6%B3%A2%E4%BC%A0%E6%84%9F%E5%99%A8.png"></div>

The color change of the block is controlled by the distance sensor.

Arduino coding
```c++
/**
*Do one demo in processing which can connect with Arduino
*2024/5/27
*By BUNBUN Team
**/

#define TrigPin A0                //control port
#define EchoPin A1                //return port

float Value_cm;                   //set distance variable

void setup() {
  Serial.begin(9600);            //initialize serial communication
  pinMode(TrigPin, OUTPUT);      //set TrigPin pin as output mode
  pinMode(EchoPin, INPUT);       //set EchoPin pin as input mode
}

void loop() {
  // put your main code here, to run repeatedly:
  digitalWrite(TrigPin, LOW);     //initialize control pin
  delayMicroseconds(2);           //hold for 2 microseconds
  digitalWrite(TrigPin, HIGH);    //deliver a high level to the control pin
  delayMicroseconds(10);          //hold for 10 microseconds
  digitalWrite(TrigPin, LOW);     //initialize control pin
  Value_cm = float(pulseIn(EchoPin,HIGH)*17)/1000;   //convert high-level pulse duration to distance

  //Serial.print(Value_cm);    //display the distance on serial monitor
  //Serial.println("cm");  //write 'cm' after the distance and do a line break
  int Val = Value_cm;
  Serial.write(Val);
  delay(1000);    //delay 1000 milliseconds
}
```
Processing coding
```java
/**
*Do one demo in processing which can connect with Arduino
*2024/5/27
*By BUNBUN Team
 * Java Exmples/Libraries/Serial/SimpleRead
**/

import processing.serial.*;

Serial myPort;  // Create object from Serial class
int val;      // Data received from the serial port

void setup() 
{
  size(200, 200);
  // I know that the first port in the serial list on my mac
  // is always my  FTDI adaptor, so I open Serial.list()[0].
  // On Windows machines, this generally opens COM1.
  // Open whatever port is the one you're using.
  String portName = Serial.list()[1]; //Make changes based on your port
  myPort = new Serial(this, portName, 9600);
}

void draw()
{
  if ( myPort.available() > 0) {  // If data is available,
    val = myPort.read();         // read it and store it in val
  }
  background(255);             // Set background to white
  if (val > 15) {              // If the serial value is 0,
    fill(#66CCFF);                   // set fill to black
  } 
  else {                       // If the serial value is not 0,
    fill(204);                 // set fill to light gray
  }
  rect(50, 50, 100, 100);
}



/*

// Wiring / Arduino Code
// Code for sensing a switch status and writing the value to the serial port.

int switchPin = 4;                       // Switch connected to pin 4

void setup() {
  pinMode(switchPin, INPUT);             // Set pin 0 as an input
  Serial.begin(9600);                    // Start serial communication at 9600 bps
}

void loop() {
  if (digitalRead(switchPin) == HIGH) {  // If switch is ON,
    Serial.write(1);               // send 1 to Processing
  } else {                               // If the switch is not ON,
    Serial.write(0);               // send 0 to Processing
  }
  delay(100);                            // Wait 100 milliseconds
}

*/
```
<div><img width="1000" src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/0d3dee4fc454ca8077da84aee6cac81223d3c702/images/processing/PROCESSING-ARDUINO.gif"></div>