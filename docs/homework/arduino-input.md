<h1 style="color: #e19cab;">Arduino Input</h1>

<h2 style="color: #e19cab;">Analog circuit connection：</h2>
<img src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/04758b785598f4858a7408c46e20ffe9acacac30/images/Arduino/%E6%9C%80%E7%BB%88input.jpg" alt="Arduino-input" width="1200">

<h2 style="color: #e19cab;">Efect 1 GIF Animation：</h2>
<img src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/411de6c3bfdc343ab1dd1dd4adec564335c6f46b/images/Arduino/%E6%95%88%E6%9E%9C%E4%B8%80.gif" alt="Arduino-input" width="1200">

<h2 style="color: #e19cab;">Efect 2 GIF Animation：</h2>
<img src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/411de6c3bfdc343ab1dd1dd4adec564335c6f46b/images/Arduino/%E6%95%88%E6%9E%9C%E4%BA%8C.gif" alt="Arduino-input" width="1200">


<h2 style="color: #e19cab;"> We have selected two effects for this Arduino Input assignment：</h2>
（1） When the distance between the object and the ultrasonic detector is less than 50cm, the WS2812 light ring starts to emit light in turn in sequence; When the distance is greater than 50cm, the light ring goes out.

<h3 style="color: #e19cab;"> Physical connection diagram：</h3>

<img src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/861f8db1b5f6f992ca08130d57731b976bac2727/images/Arduino/1.gif" alt="Arduino-input" width="1200">
<h3 style="color: #e19cab;"> Code：</h3>

```c++
/**
*This is the first effect of Arduino Input interactive
*2024/5/30
*By BUNBUN Team
**/
#include <Adafruit_NeoPixel.h> //This line includes the Adafruit_NeoPixel library, which is used for controlling WS2812 LED rings.

#define TRIG_PIN 2 //The trigger pin of the ultrasonic sensor, connected to digital pin 2 on the Arduino.
#define ECHO_PIN 3 //The trigger pin of the ultrasonic sensor, connected to digital pin 3 on the Arduino.
#define LED_PIN 6 // The data pin for the WS2812 LED ring, connected to digital pin 6 on the Arduino.
#define NUM_LEDS 8 // The number of LEDs on the WS2812 LED ring, which is 8 in this case.

Adafruit_NeoPixel strip(NUM_LEDS, LED_PIN, NEO_GRB + NEO_KHZ800); //NUM_LEDS: Specifies the number of LEDs on the LED ring.LED_PIN: Specifies the Arduino pin number connected to the data pin.NEO_GRB + NEO_KHZ800: Specifies the color arrangement and frequency of the LED ring.

void setup() {
  Serial.begin(9600);
  pinMode(TRIG_PIN, OUTPUT);
  pinMode(ECHO_PIN, INPUT);
  strip.begin();
  strip.show(); // Initialize the LED ring
}

void loop() {
  long duration, distance;

  // Send ultrasonic pulse
  digitalWrite(TRIG_PIN, LOW);
  delayMicroseconds(2);
  digitalWrite(TRIG_PIN, HIGH);
  delayMicroseconds(10);
  digitalWrite(TRIG_PIN, LOW);

  // Calculate ultrasonic round-trip time
  duration = pulseIn(ECHO_PIN, HIGH);

  // Convert time to distance, unit: centimeters
  distance = duration * 0.034 / 2;

  // Print distance to serial monitor
  Serial.print("Distance: ");
  Serial.print(distance);
  Serial.println(" cm");

  // If distance is less than 50 centimeters, sequentially light up LEDs on the LED ring
  if (distance < 50) {
    for(int i=0; i<NUM_LEDS; i++) {
      strip.setPixelColor(i, strip.Color(34, 100, 230)); // Set color to blue
      strip.show(); // Update LED ring display
      delay(100); // Wait for a while
    }
  } else {
    strip.clear(); // Clear the LED ring
    strip.show(); // Update LED ring display
  }

  // Wait for a while before next measurement
  delay(1000);
}

```
（2） When the distance between the object and the ultrasonic detector is greater than 50cm, the first lighting effect will be displayed: the WS2812 light ring will continue to flash;
When the distance is less than 50cm, display the second lighting effect: the light ring starts to light up in sequence
<h3 style="color: #e19cab;"> Physical connection diagram：</h3>
<img src="https://github.com/NexMaker-Fab/2024ZWU-IS-8-BUNBUN/raw/861f8db1b5f6f992ca08130d57731b976bac2727/images/Arduino/2.gif" alt="Arduino-input" width="1200">

<h3 style="color: #e19cab;"> Code：</h3>

```c++
/**
*This is the second effect of Arduino Input interactive
*2024/5/30
*By BUNBUN Team
**/
#include <Adafruit_NeoPixel.h>

#define TRIG_PIN 2
#define ECHO_PIN 3
#define LED_PIN 6 // Data pin for WS2812 LED ring
#define NUM_LEDS 8 // Number of LEDs on the LED ring

Adafruit_NeoPixel strip(NUM_LEDS, LED_PIN, NEO_GRB + NEO_KHZ800);

void setup() {
  Serial.begin(9600); // Initialize serial communication at 9600 baud
  pinMode(TRIG_PIN, OUTPUT); // Set the trigger pin as output
  pinMode(ECHO_PIN, INPUT); // Set the echo pin as input
  strip.begin(); // Initialize the LED strip
  strip.show(); // Initialize the LED strip
}

void loop() {
  long duration, distance;

  // Send ultrasonic pulse
  digitalWrite(TRIG_PIN, LOW);
  delayMicroseconds(2);
  digitalWrite(TRIG_PIN, HIGH);
  delayMicroseconds(10);
  digitalWrite(TRIG_PIN, LOW);

  // Calculate the round trip time of the ultrasonic pulse
  duration = pulseIn(ECHO_PIN, HIGH);

  // Convert time to distance, unit: centimeters
  distance = duration * 0.034 / 2;

  // Print distance to the serial monitor
  Serial.print("Distance: ");
  Serial.print(distance);
  Serial.println(" cm");

  // If distance is less than 50 centimeters, light up the LED ring one by one
  if (distance < 50) {
    for(int i=0; i<NUM_LEDS; i++) {
      strip.setPixelColor(i, strip.Color(34, 100, 230)); // Set color
      strip.show(); // Update LED ring display
      delay(100); // Wait for a while
    }
  }
  // If distance is greater than 50 centimeters, blink the LED ring once per second for 5 seconds
  else {
    for(int i=0; i<5; i++){
      strip.fill(strip.Color(34, 100, 230)); // Light up LED ring
      strip.show();
      delay(500);  // Light for 500 milliseconds
      strip.clear(); // Turn off LED ring
      strip.show();
      delay(500);  // Dark for 500 milliseconds
    }
  }
}

```