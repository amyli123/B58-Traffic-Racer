# Traffic Racer

## Prerequisites

* MARS MIPS simulator (requires Java)

## Configuration

Open MARS. Under `Tools`, select the `Bitmap Display` and `Keyboard and Display MMIO Simulator` windows, and click `Connect to MIPS`.

#### Bitmap Display

* Base Address for Display: 0x10008000
* Unit width in pixels: 4
* Unit height in pixels: 4
* Display width in pixels: 256
* Display height in pixels: 256

Other display sizes will work as well as long as the ratio of unit width/height to display width/height is 1:64. 

E.g. unit width/height = 8 and display width/height = 512.

## Run the Program

Under `Run`, click `Assemble`. Then, click `Go` (or the green play button) to run the program.

## How to Play

### Game Controls

Enter game input by typing characters inside the `KEYBOARD` section of the `Keyboard and Display MMIO Simulator`.

#### Starting Screen
* `p` start level

#### During Levels
* `w` speed up (4 speeds total)
* `s` slow down
* `a` move left
* `d` move right

#### Game Over Screen
* `r` retry

To quit at any point in the game, press `q`.

### Game Features

* The number of __remaining lives__ is displayed in the top left corner. At the beginning of each level, you are given 6 lives. Everytime you collide with another car or the road boundary, you lose a life and your progress is reset. Once you run out of lives, it's game over and you will have the choice to restart the game or quit.
* A __progress bar__ can be found at the top right of the screen. The level is over once the bar is completely filled. (The higher your speed, the faster the bar fills up)
* At each level, there are cars moving in different directions and at different speeds.
* There are 2 levels in total. The second level features cars with higher speeds and spawn rates.

### Pickups

Get pickups by colliding with them.

* Extra Lives `+` : Recovers 1 life (half a heart).
* Invincibility `*` : Turns your car invincible. No lives will be lost if a collision occurs in this state.

## Gameplay

<table><tr>
<td><img src="/images/startmenu.png"></td>
<td><img src="/images/gameplay.png"></td>
</tr></table>
<table><tr>
<td><img src="/images/level1complete.png"</td>
<td><img src="/images/level2complete.png"</td>
<td><img src="/images/gameover.png"</td>
</tr></table>
