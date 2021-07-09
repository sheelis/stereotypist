# Stereo Typist

> TODO: come up with a better project name

The Swiss chocolate of field keyboards: a wireless keyboard equipped with multiple forms of control, connection and input.

The reason for this invention is to have a Human Interface Device (HID) coded for coders and made for makers and also all-round human-to-device-interfacers.

This project is currently under development and some of the following brainstorm ideas are still somewhere between impossible, awesome and experimental.

## Functions 

- CONNECTIONS
  - BT: switch between 5 BT devices to control
  - WIFI: talk to LAN/WAN, change settings, SSH, 
  - micro USB OTG: for arduinos, USB drives, etc, also works as wired kb
  - micro USB: for charging (separate so that can charge and use OTG at same time)

- BUILD
  - Aluminum CNC milled casing
  - Rounded, rugged and protected
    - prevent heat/dust/dirt/water accumulation and damage
    - unlikely to be waterproof, but should be splash-proof and survive in the back pocket of a skateboarder for a week.
  - Customizable
    - Replaceable bottom plate sections with one or up to 4 of these:
      - thin magnet strip - lets you stick your keyboard to your car, robot or other solid and ferrous surface
      - Suction cups? - stick the kb to non-ferrous solid surfaces too!
      - Velcro (R) - that thing that sticks to sweaters. Lets you mount the keyboard to your sleeves, pockets, chest
      - Belt clip - for the 90's kids
      - Non-slip rubber feet - for classic and boring desktop use, except there are material and thickness choices (soft silicone cube or a cut-off from an old inner tube: up to you)


- POWER
  - Rechargeable batteries - should last for a week without recharge (fill blast during office hours)
    - use 2 flat phone batteries
      - maybe a few 1000 mAh nokia batteries for 10$ (they are even hot-replaceable)
    - report battery status to main OS
    - maybe a waterproof, magnetic charging socket?


- MOUSING
  - track pad, or some other cursor move feature (just a mouse laser?)
  - joysticks for scroll, pan, zoom - (programmable)

- KEYS
  - light and snappy buttons for text
  - clicky, defined buttons for Space, shift, ctrl, alt, tab ..
  - loudest, hardest buttons for ENTER, BCKSPC, CAPS, ESC
  - low profile caps

- FEEDBACK
  - MINI OLED or TFT
    - battery, device, mode, WIFI, sensor readings
  - LED
    - ON/OFF - always on

- LAYOUT
  - LEFT: is the MASTER and is intended to be sufficient for most non-typing tasks
    - it is the chosen one since it has WASD keys and can give most functions for those who like the half keyboards for gaming
    - all sensors
  - RIGHT: slave to the right but can also be used alone (why though?, maybe for gamers who hold the mouse in the left hand and move with the right?)
    - extra batteries (if the split kb is joined by a cable)
  - BOTH:
    - try both staggered and ortho versions and maybe something in the middle. TODO: Trace natural fingertip movements
    - take advantage of thumbs and index fingers more
    - leave the left pinky for media controls etc


- EXTRAS
  - modes:
    - switch between customizable modes of operation (mostly for macro keys)
  - media:
    - rotary encoders for volume mixer (programmable) - can be enabled with a function key
  - [fingerprint scanner?](https://www.aliexpress.com/item/33053655412.html?spm=a2g0o.productlist.0.0.c7d068c0NfLHIT&algo_pvid=b188a61c-a120-495b-b27b-4782ebb96957&algo_exp_id=b188a61c-a120-495b-b27b-4782ebb96957-3) 
  - Macros, but super powerful:
    - run local or remote commands
    - dynamic macros - react to inputs
  - build:
    - built-in magnets for snapping together for storage and with armrests
    - changeable bottom plate - attach velcro, MOLLE, magnetic, or legged bottom plates or make your own
    - small led flashlight for each side
      - adjustable angle and color/brightness
  - super experimental:
    - mini helping hand / gripper - for holding a small object - like a pen, ruler etc
    - IR blaster mode. boom! now your keyboard can control the TV and AC from your home row and with rotary dials. record and store IR macros
    - multimeter functions: VDC, R, Cap, Amps, detachable probes
    - small jack for walkie talkie microphone and earpiece (for wlan chat)
  - sensors: display on mini screen and send to PC the readings of:
    - distance measure from a ToF sensor
    - thermal imaging sensor
    - compass, accelerometer (can help to measure slopes and map areas)
    - mini scale + hx711 on one key (measure weight of small objects)
    


## Possible approaches:

### Corne

- https://github.com/foostan/crkbd
- https://www.youtube.com/watch?v=CpmQc1aTDpA

### Pro micro (atmega 32u4)

- an arduino that can be set to HID mode over USB

### ESP-32 - BT

- [feather adafruit bluetooth](https://learn.adafruit.com/custom-wireless-bluetooth-cherry-mx-gamepad/software)
- [ESP32-BLE-Keyboard software]https://github.com/T-vK/ESP32-BLE-Keyboard
- https://www.hackster.io/brian-lough/diy-bluetooth-macro-keypad-d30934#toc-other-tips-for-the-library-5
- https://gist.github.com/manuelbl/66f059effc8a7be148adb1f104666467
- [gamepad](https://www.youtube.com/watch?v=dODmsoAu0D4)

### Pi Zero W

> TODO: test boot up times with a light OS to see if it will do

- [set pi to hid mode?](https://retropie.org.uk/forum/topic/15535/turn-my-raspberry-pi-0w-into-a-bluetooth-hid-gamepad/2)
- [USB HID mode](https://gndtovcc.home.blog/2020/04/17/turn-your-raspberry-pi-zero-into-a-usb-keyboard-hid/)
- https://stackoverflow.com/questions/49139136/emulate-a-gaming-device-raspberry-pi-zero


### Any arduino + HC-05/06

- [flash it with an ftdi](https://www.youtube.com/watch?v=y8PcNbAA6AQ)
- https://www.instructables.com/3-Bluetooth-HID-Module-HC05-With-RN42-Firmware/
- https://www.kobakant.at/DIY/?p=3310

### BLE-nano

- https://inductive-kickback.com/projects/nanokeys/
- https://github.com/bitbank2/BLE_Keyboard/blob/master/BLE_Keyboard.ino


### Other useful info

- stm8 mini charge kb https://www.instructables.com/When-Cheery-Meet-Logitechdiy-a-Wireless-Mechanical/
- https://qmk.fm/
- https://www.instructables.com/Arduino-Laptop-Touchpad/




## External resources

CAD:
- [Kailh choc switches on grabcad](https://grabcad.com/library/kailh-choc-low-profile-switch-1) by Stephan Park
- [low profile keycaps on grabcad](https://grabcad.com/library/kailh-lp-choc-keycap-for-corne-1) by Stephan Park
- [joystick on grabcad](https://grabcad.com/library/joy-stick-for-arduino-1) by Anirudh Bhalekar

PCB:
- [keyswitch footprints](https://github.com/daprice/keyswitches.pretty)
- [pi zero W footprints](https://github.com/AchimPieters/KiCad-Templates)


