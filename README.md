# Nuntendo-Switchn-t-

## BACKGROUND
Hello hello hello person who has stumbled onto my GitHub repository, I'm so glad that you're here, before I go into my project some background on the name because I find it funny - I was initially thinking of designing a gaming console that runs existing games (like a switch)when I realised that that's too complex for me as of now ,so we improvise adapt overcome around here presentingggg the <ins> NUNTENDO SWITCHN'T <ins>.

It is a gaming console containing games coded by yours truly, meee. The name itself is a pun and an abbreviation for nun (nothing)like a Nintendo, not a switch. Throughout this repository you will see my attempt at running a console that runs basic games such as pong,tetris,snake and maybe(if time permits and my coding abilities prevail) a subway surfer inspired endless runner.

Watch as I try to build a functional handheld gaming console on a budget and hopefully end up with something that doesn't spontaneously disappoint me or go kaboom.

## CASE
<img width="416" height="280" alt="changed material" src="https://github.com/user-attachments/assets/3c1a2a9b-06ab-438f-ae22-0bc7862954d4" />

This is what the 3d case looks like. It will also have a display (the case has a little display holder area so as to support the display and hold it in place, it will then be connected to the PCB through wires). This is present in

## HARDWARE
The microprocessor I chose for this device is a **raspberry pico**, I chose this because of the number of pins that were available,since I wanted to have 10 buttons so as to truly capture the look of a switch. It uses an **ST7789 TFT display**, which allows for more colorful images to be displayed. A **LiPo battery** so as to store energy and ensure that it does not have to always stay connected to a computer, **10 push buttons** to allow for interaction with the device, a **DF player** which reads the music stored in a **micro SD card** and plays it through a speaker (this allows for soundtracks as otherwise it would take too much storage and not allow for individual soundtracks).It also has a passive buzzer for in game sound effects and protective components.  

### Materials Required
List of Required Parts:-
1. Raspberry Pi Pico 
2. ST7789 TFT display
3. LiPo battery
4. 10 push buttons
5. DFPlayer Mini 
6. Micro SD card 
7. Small speaker 
8. Passive buzzer 
9. Protective components (eg:- resistors, details in BOM)
10. Connecting wires 
11. Breadboard or custom PCB (refer PCB and schematic folder for PCB details)
12. Sliding switch
13. Battery charging module 

## PCB
It also uses a pcb, that is the one that is shown below

<img width="430" height="413" alt="final pcb" src="https://github.com/user-attachments/assets/48e73f3d-e9ba-46ae-8db5-cfafc8004bfe" />
<img width="455" height="371" alt="pcb final back" src="https://github.com/user-attachments/assets/66f34764-1cf6-4382-a445-391983d2c91a" />

I used a ground fill for all the ground connections (the ground net) as otherwise the connections would be incredibly messy and chaotic. 

<img width="538" height="332" alt="image" src="https://github.com/user-attachments/assets/65a340c7-3294-48ca-99b0-0b89a45b2054" />


The schematic



## Firmare
I coded the games myself in Arduino C++. The basic idea is that each game has a start function and an update function and a redraw function which allows for the respective function of each game to be called according to the player's choice of game. Each game also has its own theme (blue, green, purple and pink). I try to give the overall console a purple theme (cuz purple is my favorite color). The high scores in each game is stored alongside an identifier and retrieved as and when necessary. The console also has soundtracks, which play in the background whenever the player opens a game and also sound effects for whenever something happens in game. The long lines of code that you see with numbers and letters are C++ arrays, which represent icons and images when compiled. The firmware also allows for a mute button and a settings page. The battery level of the console as well as if it is muted or not is always displayed on top of the screen. It also plays a countdown before the start of every game. 

### GAMES
The console has four games as of now:-
> Snake
> Tetris
> Pong
> Runner
These games all have their respective icons which are displayed on the menu screen.


<img width="604" height="293" alt="image" src="https://github.com/user-attachments/assets/86713083-0694-4d05-9aa0-33d21c39f250" />


Some of the icons that are used as well as other images. 

## CONTROLS

| Screen        | Controls                                                 |
| ------------- | -------------------------------------------------------- |
| **Menu**      | A: open / X: mute /Select: settings                      |
| **Game info** | A: start / Back: menu                                    |
| **Other**     | Select: pause/resume / Back: quit to menu                |
| **Game over** | A: play again / Back: menu                               |
| **Settings**  | Up/Down: pick / Left/Right: change / Back: save and exit |

## BOM
|Item                      |Qty|Supplier       |Cost/item|Total Cost|link                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|--------------------------|---|---------------|---------|----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|Raspberry Pi Pico H       |1  |electro:kit    |$6.40    |$6.40     |https://www.electrokit.com/raspberry-pi-pico-h                                                                                                                                                                                                                                                                                                                                                                                                                   |
|TFT Display               |1  |pch butik      |$5.90    |$5.90     |https://shop.pchbutik.se/en/display/2176-13-tum-fullfaergs-skaerm-240x240-pixel.html                                                                                                                                                                                                                                                                                                                                                                             |
|DFPlayer Mini             |1  |electro:kit    |$5.90    |$5.90     |https://www.electrokit.com/mini-mp3-spelare-microsd                                                                                                                                                                                                                                                                                                                                                                                                              |
|Micro SD card             |1  |buyersblub     |$5.80    |$5.80     |https://buyersclub.se/produkt/pny-technologies-pny-performance-plus-flash-minneskort-32-gb-microsdhc?utm_source=google&utm_medium=cpc&gad_source=1&gad_campaignid=21655775898&gbraid=0AAAAABVII9b4MrMbIP7lZco0kvsZJZ3Vy&gclid=CjwKCAjwo5bXBhAEEiwAkgpgXIUCHlNceiSwIhqjqpALN88NGdgrhMvW-iIIccG-YEL_LzI1m4LPGhoCMtkQAvD_BwE                                                                                                                                        |
|Li ion battery            |1  |Batteriexperten|$6.90    |$6.90     |https://www.batteriexperten.com/sv/artiklar/midland-btnext-batteri,-3.7v,-950-mah.html?utm_source=google&utm_medium=cpc&utm_campaign=AR%20-%20SE%3A%20Standard%20Shopping%20-%20Rest%20-%20Batterier&utm_id=23913167677&gad_source=1&gad_campaignid=23913167677&gbraid=0AAAAAD9zpgyFFHinEfA34MnCptPDJ_1fl&gclid=CjwKCAjwl4HXBhAjEiwAHlpWhFjRTNh2fGXY2M733engzB79sRJL6pDqx75AQ0mQLGFw3JaC4VQvjhoClzMQAvD_BwE                                                      |
|Miniature speaker         |1  |electro:kit    |$2.80    |$2.80     |https://www.electrokit.com/miniatyrhogtalare-8ohm-2w-20x30x6.8mm                                                                                                                                                                                                                                                                                                                                                                                                 |
|Charger module            |1  |Ali Express    |$1.50    |$1.50     |https://www.aliexpress.com/item/1005012452644598.html?invitationCode=T01LNFg5YnFhWU85citoZ1pjeUlwZHorbjc1Ri9hdW1wMmp6RnFVOXR5aWVQemFTZUJrNWVWT0s1MU1hdTAyWg&channel=nnGlobal&srcSns=sns_Copy&sourceType=570&spreadType=socialShare&social_params=61662831660&bizType=ProductDetail&spreadCode=T01LNFg5YnFhWU85citoZ1pjeUlwZHorbjc1Ri9hdW1wMmp6RnFVOXR5aWVQemFTZUJrNWVWT0s1MU1hdTAyWg&shareId=61662831660&businessType=ProductDetail&platform=AE&afSmartRedirect=y|
|Slide switch              |1  |electro:kit    |$1.05    |$1.05     |https://www.electrokit.com/skjutomkopplare-1-pol-on-on-smd-2.54mm                                                                                                                                                                                                                                                                                                                                                                                                |
|Buttons (tactile switches)|1  |electro:kit    |$1.25    |$1.25     |https://www.electrokit.com/tryckknapp-pcb-6x6x4.3mm-svart                                                                                                                                                                                                                                                                                                                                                                                                        |
|pcb                       |1  |jlcpcb         |$4.00    |$4.00     |https://jlcpcb.com/                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|BC557B Transistor         |1  |electro:kit    |$1.25    |$1.25     |https://www.electrokit.com/en/bc557b-to-92-pnp-50v-100ma                                                                                                                                                                                                                                                                                                                                                                                                         |
|100 uF capacitor          |1  |electro:kit    |$1.12    |$1.12     |https://www.electrokit.com/en/el.lyt-smd-100uf-6.3v-85c-5x5.2mm                                                                                                                                                                                                                                                                                                                                                                                                  |
|Screw PH M3x25            |1  |electro:kit    |$1.65    |$1.65     |https://www.electrokit.com/en/skruv-ph-m3x25                                                                                                                                                                                                                                                                                                                                                                                                                     |
|Estimated total shipping  |1  |               |         |$6.00     |                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |


## CREDITS
This was created as a hack club project for halflife, the code has been written by me.
All the images present in my firmware have been taken from different sources online. 



