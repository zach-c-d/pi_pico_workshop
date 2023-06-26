# notes for planning the pi pico workshop!

## workshop resources & research notes

- wiki page: https://wiki.hacklab.to/Arduino_for_Beginners_with_A-Train_and_Zack

- beginner projects with excellent documenation: rpf.io/pico-intro
- [servo library](https://pypi.org/project/micropython-servo/)
  - alternative: servo class: https://how2electronics.com/how-to-control-servo-motor-with-raspberry-pi-pico/
- saving a python script "on the pico filesystem" as `main.py` will cause the pico to automatically run that script on boot.

---

## workshop skeleton

1. introduction to computers
   - terminology
2. get people setup with tools
   - how to install the software
   - how to connect the computer
3. get people setup with a basic example to hack on
   - blink example
   - button example
   - servo example
     - servo with zerostop example

---

## introduction to computers

### What is a Raspberry Pi Pico?

### What is a Microcontroller?

- a cheap computer that only runs one program, and starts it automatically when it turns on

#### Why use a microcontroller

- power effecient
  - doesn't have a regular operating system or other programs taking up "cycles" of the processor.
- great for precise and fast timing -- on the order of nanoseconds
  - second, millis, micro, nano --> ( 0.000001 seconds)

### Why use a Raspberry Pi

- The RaspberryPi organization is focused on education
  - Their products are well documented
- RaspberryPi is a popular brand, so there is a large community of tinkerers using these boards
  - makes googling easier
    - stack overflow answers
    - reddit answers

## How to start coding with the Pico?

- googlefu
- software
  - Thonny
  - libraries

### Google Fu

- how to structure google search:

> `MicroPython` + `[Specific Error Message]`

- other great keywords: `stackoverflow` `reddit` `RP2040`

## software

### thonny

### libraries
