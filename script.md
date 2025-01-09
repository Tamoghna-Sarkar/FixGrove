# GROVEPI ISSUE RESOLUTION

## REFLASH YOUR SDs and FOLLOW THE EXACT STEPS:

### Step1:

ssh into your rpi

### Step2:

sudo rm -rf Dexter

this just removes the Grove stuff you have installed previously

### Step3:

curl -KL https://raw.githubusercontent.com/Tamoghna-Sarkar/FixGrove/main/grove-setup.sh | bash

### Step4:

cd /Dexter/GrovePi/Firmware

sudo raspi-config nonint do_spi 1
sudo raspi-config nonint do_i2c 1
./firmware_update.sh

### Step4: TEST YOUR GROVEPI w your LED

Attach the LED to Digital Pin 4 on the GrovePi (you can change pin number according to where

you attach yours, I used 4)

cd  Dexter/GrovePi/Software/Python

python grove_led_blink.py

and you should see your LED blinking.

NOW, GET STARTED WITH YOUR LAB2
