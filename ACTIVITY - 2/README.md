- Description of the Activity 

  In this laboratory activity, we expanded the previous running light project by using analog signals.
The same running light logic was applied, but this time the brightness of the LEDs is controlled using analogWrite().

  This activity helps us understand analog to digital signal conversion and how the map() function is used in Arduino.

- Circuit Setup

  The LEDs are connected to digital pins 8 to 12 of the Arduino.
Each LED is connected in series with a resistor and all grounds are connected to the GND pin of the Arduino.

  (The breadboard diagram for this activity is included in this folder.)

- Code Explanation

  An array is used to store the LED pin numbers from 8 to 12, which makes the code more organized.
A while() loop is used to set the pin modes and control the LED sequence.

  The map() function converts the input value into a range that can be used by analogWrite().
The LEDs turn ON with increasing brightness from pin 12 to pin 8, with a 1-second delay.
After all LEDs reach maximum brightness, they turn OFF one by one in the same order.

  The function analogWrite() is used to control the brightness of each LED.
