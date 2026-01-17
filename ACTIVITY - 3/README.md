- Description of the Activity

  In this laboratory activity, we worked with basic sensor components used in IoT systems.
A simple fire sensor implementation was created using a thermistor and a photoresistor connected to an Arduino.

  The system detects fire by checking temperature and brightness levels. When both threshold limits are reached, a red LED (and optional buzzer) is activated to notify the user.

- Circuit Setup

   - Thermistor is connected to analog pin A0
   - Photoresistor is connected to analog pin A2
   -  Red LED is connected to digital pin 12
   -  All components share a common GND
   -  A breadboard diagram is included in this folder
 

- Program Logic and Code Explanation

 The pin numbers are handled using #define for better code readability.
The threshold values are declared using const variables.

- Separate functions are used to read:

  - Temperature (in Celsius) from the thermistor
  - Brightness value from the photoresistor

- The program continuously checks if:

  - Temperature is 50°C or higher, and
  - Brightness value is 220 or higher

 If both conditions are met, the red LED blinks rapidly to indicate a possible fire.
If connected, the buzzer also activates using the same pin as the LED.
