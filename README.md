# StereoTypist

A fully wireless bluetooth split keyboard with customization and modern needs in mind.

The reason for this invention is that mechatronics engineers often code, control and interact with IOT devices and their terminals via keyboards, but conventional keyboards are too inconvenient as they are big, require to be on a surface and surface space is often taken up by tools or wiring etc.

Chest keyboard would be a regular KB split in two and reconnected at top edges and then strapped / clipped to chest so that one could type by placing hands on ribcage.
In combination with the chest phone holder running VNC or SSH, this could be a very powerful portable terminal rig capable of 3d software applications while operator is on the move.


## Functions 

- CONNS
  - switch between 5 BT devices to control
    - must have good range!
  - wifi chip allows to upload new config files and talk to web
  - cable - maybe needed for bios stuff?

- BUILD
  - change angle of split (not full split but rather a hinge)
  - wake on touch or key combo or hover
  - easy cover or flip around to prevent dust/dirt/water/damage from mechanical work
  - easy clip on / off the chest or slide behind back
  - allow movements (bending, crouching etc)
  - harmonica strap to support hand on chest

- POWER
  - WIFI - on/off
  - lights on/off
  - on/off switch (to avoid accidental key press)
    - sleep when inactive for x seconds *programmable*
  - rechargeable batteries (last for a week at least and indicate low batteries)
    - use 2 flat phone batteries
    - report battery status to main OS

- MOUSING
  - trackpad, clit, or some other cursor move feature (just a mouse laser?)
  - joystick for scroll, pan, zoom - *programmable*

- KEYS
  - light and snappy buttons for text
  - clicky, defined buttons for Space, shift, ctrl, alt, tab ..
  - loudest, hardest buttons for ENTER, BCKSPC, CAPS, ESC
  - low profile caps

- FEEDBACK
  - MINI OLED
    - battery, device, mode, wifi
  - LED
    - ON/OFF - always on
      - show mode - color (RGB)
    - each BT device should have LED
      - blue - connected
      - yellow - assigned, idle
      - off - not yet paired


- EXTRAS
  - software for customizing keys (maybe web interface using SPIFFS of shit)
  - switch between 5 modes of operation (mostly for macro keys) *programmable*
  - encoders for volume mixer *programmable*
  - big encoder wheel  - maybe for spinning through open apps etc *programmable*
  - small led flashlight for each side
    - adjustable angle and color
  - custom keys for each hand (combine with F keys) *programmable*
    - key to start and stop a new note and save it over wifi or locally on SD card?
    - assign a web task to a button (run a url)
    - run a command


## Possible approaches:

### Corne

https://github.com/foostan/crkbd
https://www.youtube.com/watch?v=CpmQc1aTDpA

### Pro micro


### ESP-32 - BT

- https://github.com/T-vK/ESP32-BLE-Keyboard
- https://www.hackster.io/brian-lough/diy-bluetooth-macro-keypad-d30934#toc-other-tips-for-the-library-5
- https://gist.github.com/manuelbl/66f059effc8a7be148adb1f104666467

### Any arduino + HC-05/06

- https://www.instructables.com/3-Bluetooth-HID-Module-HC05-With-RN42-Firmware/
- https://www.kobakant.at/DIY/?p=3310

### BLE-nano

- https://inductive-kickback.com/projects/nanokeys/
- https://github.com/bitbank2/BLE_Keyboard/blob/master/BLE_Keyboard.ino

### Ergodone 


### other useful info

- stm8 mini charge kb https://www.instructables.com/When-Cheery-Meet-Logitechdiy-a-Wireless-Mechanical/
