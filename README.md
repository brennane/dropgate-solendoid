
# Solenoid Project



## Schematic

This is my first foray into using KiCad.  The project could probably add a 24V
TVS added to to handle voltage spikes but I don't have any on hand but can add
that later.

The U2 Block represents a USB-C Power-Delivery Module pegged to 20V output.
These are cheap.  The easy-to-find linear solenoids are 24V and so are running 
about 2/3rd power.  I spec'd a 24V 400mA for this board but we could go up to
24V 2A output without causing issues -- which is the way to get more oomph in
this design. 

I have three LEDs on the board.  One LED is telling us we have power on the +12V
rail.  One LED turns on when the input signal (in my case a 2-3sec 9V input from
a light array).  The last LED turns on when the solenoid is draining and that
will run as long as the the timer is set.

Timer.  There is a trimmer pot on the board that can sweep from about 1/2 sec to 
6 sec when we see an external signal coming in.


Use the Online viewer at <https://kicanvas.org> to
view the Schematic: [solenoid-1.kicad_sch](https://kicanvas.org/?repo=https%3A%2F%2Fgithub.com%2Fbrennane%2Fdropgate-solendoid%2Fblob%2Fmain%2Fsolenoid-1.kicad_sch)
