# Nuntendo-Switchn-t-

## BACKGROUND
Hello hello hello person who has stumbled onto my GitHub repository, I'm so glad that you're here, before I go into my project some background on the name because I find it funny - I was initially thinking of designing a gaming console that runs existing games (like a switch)when I realised that that's too complex for me as of now ,so we improvise adapt overcome around here presentingggg the <ins> NUNTENDO SWITCHN'T <ins>.

It is a gaming console containing games coded by yours truly, meee. The name itself is a pun and an abbreviation for nun (nothing)like a Nintendo, not a switch. Throughout this repository you will see my attempt at running a console that runs basic games such as pong,tetris,snake and maybe(if time permits and my coding abilities prevail) a subway surfer inspired endless runner.

Watch as I try to build a functional handheld gaming console on a budget and hopefully end up with something that doesn't spontaneously disappoint me or go kaboom.

## CASE
<img width="416" height="280" alt="changed material" src="https://github.com/user-attachments/assets/3c1a2a9b-06ab-438f-ae22-0bc7862954d4" />

This is what the 3d case looks like. It will also have a display (the case has a little display holder area so as to support the display and hold it in place, it will then be connected to the PCB through wires). This is present in

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
>Snake
>Tetris
>Pong
>Runner
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

This was created as a hack club project for halflife



