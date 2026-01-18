- Description of the Activity

  In this laboratory activity, we implemented Arduino control using FastAPI.
Python is used as a bridge between HTTP requests and Arduino serial communication to create a bi-directional system.

  FastAPI endpoints are used to control LEDs connected to the Arduino.

- Circuit Setup

  LEDs

  - Red LED → Digital pin 7

  - Green LED → Digital pin 6

  - Blue LED → Digital pin 5

  Push Buttons

  - Button 1 → Digital pin 12

  - Button 2 → Digital pin 11

  - Button 3 → Digital pin 10

  All components share a common GND.

  ( A breadboard diagram is included in this folder. )

- Program Logic and Code Explanation
  Arduino Side (Inbound Signal)

  - When "1" is received → Red LED toggles ON/OFF

  - When "2" is received → Green LED toggles ON/OFF

  - When "3" is received → Blue LED toggles ON/OFF

  All serial inputs are case-insensitive

  FastAPI Side (HTTP to Serial)

- FastAPI provides the following endpoints:

  can be red, green, or blue

  Sends:

  - "1" - Red LED

  - "2" - Green LED

  - "3" - Blue LED

- Turns ALL LEDs ON

- Turns ALL LEDs OFF

  FastAPI writes the corresponding values back to Arduino through the serial port.
