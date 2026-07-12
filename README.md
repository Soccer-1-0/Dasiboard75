# Dasiboard75

This is my attempt at creating a keyboard with 84 keys, with backlights, a rotary encoder, a slide potentiometer, a OLED screen, and a power switch, using just the 19 usable pins of a XIAO NRF52840 Plus.
<img width="1056" height="538" alt="Render" src="https://github.com/user-attachments/assets/29005a24-72f2-402f-b229-1299ea50eae3" />

## CAD
Cadding everything together was the best part, since I could easily see the results fast and I didn't have to worry about any problems later in firmware. The keys will also be colored, since there is a keyset that I sourced that provides variations of light green keys, I just didn't want to add color to every individual key. I also made custom knobs for both the slide potentiometer and the rotary encoder! Dasiy flower for the encoder!

![cad1](images/cad1.png)
![cad2](images/cad2.png)

## Schematic
My schematics are so cooked that I need three images for this. The leds took so much space, but it only takes on gpio pin. I used the japanese duplex matrix, which is why there are two keys for each column in the schematic drawing for the switiches. The duplex matrix works with scanning with the different directions of diodes to be able to double the amount of keys on a keyboard, which is the main reason I was able to make a full keyboard with less pins.
![schem1](images/schem1.png)
![schem2](images/schem2.png)
![schem3](images/schem3.png)

## PCB
The routing of this took so long, since I used a 7x7(2) matrix for it, I had to move all the switiches to make sure they all connected the same way. The routing of the leds were even worse.
![pcb1](images/pcb.png)
![pcb1](images/pcb_render.png)
![pcb1](images/pcb_render2.png)

## Firmware
Still in progress, am trying to find a way for it to work with ZMK firmware, since some of my features are not supported with ZMK, but I really want to use the energy saving ways of bluetooth of ZMK.

## Casing

## BOM
