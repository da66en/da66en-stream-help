# da66en's stream channel help

Help on using bot commands, redemptions, tips on gameplay of games played with viewer control, jukebox playlist, etc

## Jukebox

To play a song, use !jukebox command followed by a number that is the song you want to play.

An example of playing song 69 (nice):

`!jukebox 69`

Here's a list of songs and their command number:  [Playlist](jukebox.md)

To play a random song, don't provide a number

## Twitch plays (viewer control)

Sending controller inputs to the game being played is done with the !emucontrol command followed by a list of button you want to input.

Here's a list of the button inputs you can send to !emucontrol

| Bot command | Description |
|---|---|
LEFT | Left on the d-pad
RIGHT | Right on the d-pad
UP | Up on the d-pad
DOWN | Down on the d-pad
L1 | Left shoulder button
R1 | Right shoulder button
A | A button
B | B button
X | X button
Y | Y button
SELECT | Select button
START | Start button

To press multiple buttons at same time, use the + character to chain multiple buttons toggether.  For example, this will press A button and LEFT d-pad at the same time:

`!emucontrol LEFT+A`

To press a button longer, use the + character to add multiple of the same commands.  For example, this will hold A an LEFT for one cycle and then hold LEFT for two more cycles (note, all inputs start at the same cycle regardless of what position the are in the command):

`!emucontrol LEFT+LEFT+LEFT+A`

To press send one chain of inputs followed by a seperate chain of inputs, add a space between the commands.  For example, this will send a LEFT and A, followed by a UP and B, followed by a START:

`!emucontrol LEFT+A UP+B START`