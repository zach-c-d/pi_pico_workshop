# notes for planning the pi pico workshop!

skip to button for most up to date notes.

## workshop resources & research notes

- wiki page: https://wiki.hacklab.to/Arduino_for_Beginners_with_A-Train_and_Zack

- beginner projects with excellent documenation: rpf.io/pico-intro
- [servo library](https://pypi.org/project/micropython-servo/)
  - alternative: servo class: https://how2electronics.com/how-to-control-servo-motor-with-raspberry-pi-pico/
- saving a python script "on the pico filesystem" as `main.py` will cause the pico to automatically run that script on boot.
- pyb -- specific for the "py board" and is not compatible with the pi pico

  - many of the methods in `pyb` are available in the `machine` library for MicroPython

- 5v rails on raspi pico
  - VBUS is the micro-USB input voltage, connected to micro-USB port pin 1. This is nominally 5 V (or 0 V if the USB is not connected or not powered).
  - VSYS is the main system input voltage, which can vary in the allowed range 1.8 V to 5.5 V, and which is used by the on-board SMPS (switch mode power supply) to generate the 3.3 V for the RP2040 and its GPIO.
  - [pi pico datasheet](https://datasheets.raspberrypi.org/pico/pico-datasheet.pdf)

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
- quick video with animation of what writing to a register looks like: https://youtu.be/3FLxA-Owgpw?t=89

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

### sensors and actuators

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

-

### libraries

- thonny package manager
- [servo library](https://pypi.org/project/micropython-servo/)

---

## on-board preloaded examples

- main.py with no examples, only comments
- Readme with links to
  - resources
  - pin out diagram
- arduino lab for micropython

```python

# Welcome to your pi pico's main program file -- main.py !!
#
# When it turns on, the Pi Pico will execute any
# code in a file named main.py in it's storage.
#
# Anything you put in this file will run automatically!
#

#
# library includes
#

#
# global variable declarations
#

#
# definitions
#

# main loop



```

---

## action items

- preload directory of example file on pi picos
  - blink example
  - button example
  - servo library
- for servo library --
  - have preloaded servo library commented out
  - get partipants to install servo library through thonny package manager
  - get participants to write `include` command for the servo library they just installed
  - in case of difficulty or internet issues, they can uncomment the preloaded servo library and continue with driving the servo.

---

## workshop flow

### strategy

start very high level and abstracted, just the basic **practical** knowledge necessary to do the exercise

introduce specifics and theory in small bits -- after exercise. practical experience gives theory context.

intro -> exercise -> theory

### schedule

- get power! wire led. wire button
- get code! blink led. listen to button. toggle led.
- get claw! install library. move claw. assemble claw. control claw with button.

#### intro

- what is this thing
  - it's a small computer
  - it has a usb port
  - it has lots of pins
  - lets connect it to our computers
- what are all its pins
  - some of the pins are power (3v3, 5v, GND)
  - some of the pins are for control
    - we can write software to do things like
      - toggle them on and off
      - listen to them and record their voltage amounts
- what is this other thing
  - it's called a "breadboard"
  - its for making easy electrical connects between things
  - <_diagram of how a breadboard is "wired"_>
  -

#### exercise

- wire led to board. get it to light up
- wire button in between led and board. get led to light up when button is pressed

#### theory
