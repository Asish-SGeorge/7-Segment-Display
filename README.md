# Arduino 7-Segment Display Counter

This project demonstrates how to drive a 7-segment display using an Arduino. The display counts from 0 to 9, with each digit displayed for one second. Each segment (A to G) of the display is controlled using individual digital output pins on the Arduino.

## Features

- Counts from 0 to 9 with a 1-second delay between numbers.
- Each digit is displayed using corresponding segment control.
- Easily modifiable for custom sequences or applications.
- Suitable for beginners learning to control LEDs or segments with Arduino.

## Hardware Requirements

- Arduino Uno (or compatible board)
- 7-Segment Display (Common Cathode)
- 8 Resistors (220Ω or 330Ω recommended)
- Jumper wires
- Breadboard

## Pin Configuration

Each segment is connected to an Arduino digital pin:

| Segment | Arduino Pin |
|---------|--------------|
| A       | 13           |
| B       | 12           |
| C       | 11           |
| D       | 10           |
| E       | 9            |
| F       | 8            |
| G       | 7            |
| H (Decimal Point or Extra LED) | 6 |

> Note: Segment `H` is optional and is not used in this project.

## Installation

1. Clone this repository:
    ```bash
    git clone https://github.com/Asish-SGeorge/arduino-7segment-counter.git
    ```

2. Open the `.ino` file in the Arduino IDE.

3. Connect your hardware as per the pin configuration.

4. Upload the code to your Arduino board.

## Usage

Once uploaded, the 7-segment display will count from 0 to 9, displaying each digit for one second before moving to the next.

## Code Structure

- Each digit (0–9) is implemented as a separate function (`zero()`, `one()`, etc.).
- `setup()` initializes all segment pins as outputs.
- `loop()` cycles through all the digit functions in sequence with a 1-second delay.

## License

This project is licensed under the MIT License.

---

Feel free to contribute or modify this project to add more features like button control, countdown timers, or multi-digit display support.
