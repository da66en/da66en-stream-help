# da66en's stream channel help

Help on using bot commands, redemptions, tips on gameplay of games played with viewer control, jukebox playlist, etc

## Jukebox

To play a song, use !jukebox command followed by a number that is the song you want to play.

An example of playing song 69 (nice):

`!jukebox 69`

Here's a list of songs and their command number:  [Playlist](jukebox.md)

To play a random song, don't provide a number

## Twitch plays (viewer control)

Sending controller inputs to the game being played is done with the !emu command followed by a list of button you want to input.

Here's a list of the button inputs you can send to !emu

| Bot command | Description |
|---|---|
L | Left on the d-pad
R | Right on the d-pad
U | Up on the d-pad
D | Down on the d-pad
L1 | Left shoulder button
R1 | Right shoulder button
A | A button
B | B button
X | X button
Y | Y button
SEL | Select button
STA | Start button

To press multiple buttons at same time, use the , character to chain multiple buttons toggether.  For example, this will press A button and LEFT d-pad at the same time:

`!emu L,A`

To press a button longer, use the , character to add multiple of the same commands.  For example, this will hold A an LEFT for one cycle and then hold LEFT for two more cycles (note, all inputs start at the same cycle regardless of what position the are in the command):

`!emu L,L,L,A`

You could also simplify this by using a ^ character followed by a number to indicate to repeat (or multiply) that command that number of times.  Here is a repeat of the previous command using this multiplier command:

`!emu L^3,A`

To repeat a command, use the * operand at end of the expression and the number after operand specifies how many times to repeat the command.  For example, here is how to send the above example 3 times:

`!emu L^3,A*3`

To press send one chain of inputs followed by a seperate chain of inputs, add a space between the commands.  For example, this will send a LEFT and A, followed by a UP and B, followed by a START:

`!emu L,A U,B STA`

To expand on the previous example, this well senda  LEFT and A, followed by a LEFT and A, followed by UP and B, followed by a START, followed by a START:

`!emu L,A*2 U,B STA*2`

Here's some extra help for specific games:
* [SNES Sim-City](snes_simcity.md)