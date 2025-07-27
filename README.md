
# Button Controlled LEDs

This is a simple Arduino project that controls three LEDs using three push buttons. Each button toggles the ON/OFF state of its corresponding LED. It demonstrates basic digital input and output control using an Arduino board.

## Requirements

* Arduino Uno (or compatible board)
* 3 push buttons
* 3 LEDs
* 3 resistors (220Ω for LEDs)
* 3 resistors (10kΩ for pull-down resistors on buttons)
* Breadboard and jumper wires
* Arduino IDE

## How It Works

Each button is connected to a digital input pin. When a button is pressed, the code toggles the state of the matching LED (turns it ON if it’s OFF, and OFF if it’s ON). The code includes simple debounce logic to avoid false triggers caused by button bounce.

## Files Included

* `ButtonControlledLEDs.ino`: The Arduino sketch containing the full logic
* `3 button.png`: A visual diagram of the circuit (not required for understanding the code)

## Code Overview

```cpp
const int button1 = 2;
const int button2 = 3;
const int button3 = 4;
const int led1 = 5;
const int led2 = 6;
const int led3 = 7;
```

Each button is read in the loop. When a press is detected, a flag is used to toggle the state of the corresponding LED.

## How to Use

1. Download or clone this repository.
2. Open the `ButtonControlledLEDs.ino` file in Arduino IDE.
3. Connect the circuit using your components.
4. Upload the code to your Arduino board.
5. Press each button to toggle its respective LED.


