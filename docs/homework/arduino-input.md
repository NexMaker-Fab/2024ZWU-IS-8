<h1 style="color: #e19cab;">Arduino Input</h1>

<h2 style="color: #e19cab;"> 1.What is Arduino Input</h2>

```c++
/**
*Using ArduinoIDE for hardware interaction, the distance between the hand and the sensor determines the brightness of the LED lights
*2024/5/28
*By BUNBUN Team
*Refer to https://www.nexmaker.com/doc/5arduino/Arduino_Input.html，but changed by ourselve
**/

#define TrigPin A0    // Define the trigger pin connection of the ultrasonic sensor as A0
#define EchoPin A1    // Define the echo pin connection of the ultrasonic sensor as A1

const int LED1 = 12; // Define the pin connection of the red LED as 12
const int LED2 = 13; // Define the pin connection of the green LED as 13

int val = 0; 
// Define an integer variable val and initialize it to 0. This variable is not currently used in the code but may be used for future functionality expansion.

long distance;  // Define a long integer variable distance to store the measured distance value

int count = 0; // Define an integer variable count and initialize it to 0 to record the loop count

long duration; // Define a long integer variable duration to store the duration of the ultrasonic sensor echo

void setup() {
 // set Serial communication
    Serial.begin(115200);
    // Initialize serial communication with a baud rate of 115200.
    // This allows Arduino to communicate with the computer via serial port.
    // set pin mode
    pinMode(LED1, OUTPUT); 
    pinMode(LED2, OUTPUT); // Set the pin mode: LED1 and LED2 as output mode
    pinMode(TrigPin, OUTPUT); // Set TrigPin as output mode
    pinMode(EchoPin, INPUT);  // Set EchoPin as input mode
    // LED pins are used to control the LED lights, TrigPin is used to trigger the ultrasonic sensor to send signals, and EchoPin is used to receive ultrasonic echo signals.
    // init pin
    digitalWrite(TrigPin, LOW);
    delay(1);
    // Set the TrigPin to a low level and delay for 1 millisecond.
    // This is to initialize the ultrasonic sensor.
}

void loop() {
    Serial.println(count++);  // Print the current loop count to the serial monitor and increment count
    Serial.println(getDistance());  // Print the distance measured by the ultrasonic sensor to the serial monitor
    distance = getDistance();   // Store the measured distance in the distance variable
    Serial.println("");
    Serial.println("");    // Print two empty lines to the serial monitor
    delay(1000);    // Delay for 1 second
    // LED control logic...
}
 if(val==HIGH) //This is a conditional statement, checking if the variable val is equal to HIGH.
{
    if (distance > 500)  {
        digitalWrite(LED1, HIGH);
        digitalWrite(LED2, HIGH);//If the condition is met, i.e., if the distance is greater than 500, both LED1 and LED2 are set to a high state (turned on).
    }
    else if (distance > 200 && distance < 500) {
        digitalWrite(LED1, HIGH);
        digitalWrite(LED2, LOW);//If the condition above isn't met but this one is, i.e., if the distance is greater than 200 and less than 500, LED1 is set to a high state and LED2 is set to a low state.
    }
    else if (distance < 200) {
        digitalWrite(LED1, LOW);
        digitalWrite(LED2, LOW);//If neither of the above conditions is met, i.e., if the distance is less than 200, both LED1 and LED2 are set to a low state (turned off).
    }

}
else
{ 
    
    if (distance > 500)  {
        digitalWrite(LED1, LOW);
        digitalWrite(LED2, LOW);//If the condition is met, i.e., if the distance is greater than 500, both LED1 and LED2 are set to a low state (turned off).
    }
    else if (distance > 200 && distance < 500) {
        digitalWrite(LED1, LOW);
        digitalWrite(LED2, HIGH);//If the condition above isn't met but this one is, i.e., if the distance is greater than 200 and less than 500, LED1 is set to a low state and LED2 is set to a high state.
    }
    else if (distance < 200) {
        digitalWrite(LED1, HIGH);
        digitalWrite(LED2, HIGH);//If neither of the above conditions is met, i.e., if the distance is less than 200, both LED1 and LED2 are set to a high state (turned on).
    }
}

// The getDistance function is used to obtain the distance measured by the ultrasonic sensor
long getDistance() {
    // Trigger the ultrasonic sensor
    digitalWrite(TrigPin, LOW); // Set the TrigPin (trigger pin of the ultrasonic sensor) to a low level
    delayMicroseconds(2);  // Pause the program execution for 2 microseconds
    digitalWrite(TrigPin, HIGH); // Set the TrigPin to a high level. This action will send a high level signal of more than 10 microseconds to the ultrasonic sensor to trigger it to send ultrasonic signals.
    delayMicroseconds(10); // This line of code pauses the execution for 10 microseconds. This delay ensures that the ultrasonic sensor can receive the trigger signal and send ultrasonic signals normally.
    digitalWrite(TrigPin, LOW); // Send the trigger pulse for the ultrasonic signals

    // Receive echo signals
    duration = pulseIn(EchoPin, HIGH); // unit: microseconds. Measure the duration of the high-level pulse on the EchoPin pin using the pulseIn function. The unit is microseconds (us).
    return duration * 0.34029 / 2;         // unit: mm
    // Convert the pulse duration to distance (unit: millimeters) according to the speed of sound formula, and return the result.
}
```

<h2 style="color: #e19cab;"> 2.Physical connection diagram</h2>
<div><img width="1000" src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/aa39231dcc18a6603a8169316bbd28294a50a502/images/Arduino/Arduino%20input%20%E4%BD%8E%E7%94%B5%E5%B9%B3.gif"></div>


<h3 style="color: #e19cab;">- HIGH LEVEL INPUT</h3>
<font size="3"><h3 style="color: #e19cab;">This figure shows the high level intput of Arduino</h3></font>

·When the ultrasonic detection device detects a distance of less than 200mm, both red and green LEDs light up simultaneously

·Between 200mm and 500mm, only green LED lights up

·Distance greater than 500mm, LED light off

<div><img width="1000" src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/aa39231dcc18a6603a8169316bbd28294a50a502/images/Arduino/arduino%20input%20%E9%AB%98%E7%94%B5%E5%B9%B3%20.gif"></div>

<h3 style="color: #e19cab;">- LOW LEVEL INPUT</h3>
<font size="3"><h3 style="color: #e19cab;">This figure shows the low level intput of Arduino</h3></font>

·When the ultrasonic detection device detects a distance of less than 200mm, LED light off

·Between 200mm and 500mm, only green LED lights up

·Distance greater than 500mm, both red and green LEDs light up simultaneously


<h2 style="color: #e19cab;">3.Arduino Analogical Electronics</h2>

<font size="5"><h2 style="color: #e19cab;">- NOT CONNECTED</h2></font>

<div><img width="1000" src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c2f5a993282a3ebbc0d05ef86e9e8ac731634045/WechatIMG22194.jpg"></div>

<font size="5"><h2 style="color: #e19cab;">- CONNECTED</h2></font>

<div><img width="1000" src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/c2f5a993282a3ebbc0d05ef86e9e8ac731634045/WechatIMG22194.jpg"></div>