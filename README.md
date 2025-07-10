# Fast-and-Slow
This Arduino sketch controls two LEDs connected to pins 12 (red) and 11 (yellow) on an Arduino board, such as an Arduino Uno, to create a sequential blinking pattern. It uses variables to define timing for the LED blinks.
The sketch defines variables: redLed (pin 12), yellowLed (pin 11), slow (500ms for red LED timing), and fast (200ms for yellow LED timing). In the setup function, pins 12 and 11 are configured as outputs to control the respective LEDs.In the loop function, the LEDs follow a repeating pattern:The yellow LED blinks five times: on for 200ms, off for 200ms each time.
The red LED blinks ten times: on for 500ms, off for 500ms each time.
The sequence repeats indefinitely.

Hardware Requirements:Arduino board with digital pins 11 and 12 (e.g., Arduino Uno, Nano).
Red LED connected to pin 12 and yellow LED to pin 11, each with a current-limiting resistor (e.g., 220 ohms) to ground.

Usage:Upload the sketch to your Arduino board using the Arduino IDE.
The yellow LED will blink rapidly five times, followed by the red LED blinking slowly ten times, in a continuous loop.

Notes:The delay function controls timing, pausing the program for the specified durations (fast for yellow LED, slow for red LED).
The pattern creates a clear contrast between the rapid yellow blinks and slower red blinks.
To modify the pattern, adjust the fast or slow variables or change the number of blinks in the loop function.
The code contains a minor typo ("bbb") after a delay call, which may cause a compilation error; remove it to ensure the sketch runs correctly.
This sketch is ideal for learning Arduino digital output, timing control, and multi-LED patterns.
