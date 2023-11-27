# Blink on board LED (Arduino)

This example demonstrates how to blink an on-board LED using an Arduino. It's a basic example to illustrate digital output control.

#### Requirements and Setup
- Hardware: doppler board
- Software: Arduino Sfotware

#### Implementation

```c
void setup() {
  pinMode(LED_BUILTIN, OUTPUT); // Initialize the LED pin as an output
}

void loop() {
  digitalWrite(LED_BUILTIN, HIGH); // Turn the LED on
  delay(1000);                     // Wait for a second
  digitalWrite(LED_BUILTIN, LOW);  // Turn the LED off
  delay(1000);                     // Wait for a second
}
```

- The `setup` function configures the LED pin as an output.
- The `loop` function turns the LED on and off with a one-second delay between states.

When this code runs, the on-board LED should blink on and off every second. This example is fundamental in understanding how to control digital outputs on an Arduino board.