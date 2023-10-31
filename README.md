# diamond
eZ80 game on AgonLight
Diamond Quest is a simple game, built purely as a goal to learn  z80 assembly routines on the Agon Light, All z80 assembly, no Basic. Run around the screen, you have 30 seconds to grab as many diamonds as possible. Your high score is retained for future sessions. 
Two player (Boy and Girl) joystick support on the Console8, you can use one player with keys (the Boy)
Whilst I have done some z80 assembly in the past (ZX81 and ZX Spectrum), the Agon architecture was a bit of a learning curve, not only the way sound and graphics are handled, but also included ADL mode, where two bytes are no longer two bytes...
I am not sharing the sources just yet, as it is still very much work in progress and needs a LOT of tidying up, but happy to share a bin file if anyone wants to play it. I'd like to split out the routines into separate code modules to make life easier on other projects.
It should run on MOS/VDP 1.04RC2, but also I am running on Console8 currently 2.0.0Alpha.
The features I learned are applicable to many different game types:-
Animated sprites.
Simple collision detection.
Bitmap graphics (tiled background).
Sound FX (very simple beeps).
Keyboard control (hopefully improve when VDP allows multiple key presses to be recognised).
Joystick (ports C & D) control.
Countdown Timer (seconds).
Program speed control (generic delay routine based on z80 clock tick).
Different screens (menu, gameplay, game over dialog).
Simple transitions, vertical wipe.
High score retained between sessions, saved in prefs file.
Custom font loaded.
User defined graphic characters.
Printing coloured text at X,Y corrdinates.
Drawing rectangles (using a triangle pair).
Use of macros to neaten/simplify repeated code.
Random number generation (for placing new diamonds).
Background music player.
Two player with both joysticks.
The graphics and fonts are mostly freeware available on the internet, just used to save me time developing my own at this stage. They needed a bit of production time to get into the correct format.
I code in Sublime Text on Mac, then assemble with ez80asm on Mac, then use Jeroen Venema's hexload utility to pipe the bin file onto the Agon. It's not easy for debugging, but is quite quick to build and run on real hardware.

