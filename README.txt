This is a schematic for the PT2399 Echo/Delay IC redrawn
from the Block Diagrams provided by ElectroSmash website,
which is invaluable for understanding how the PT2399 works
and how it may be modified by users!
Thank you ElectroSmash!

https://www.electrosmash.com/pt2399-analysis

I've redrawn the Block Diagram, then laid out
the typical circuit taken from the PT2399 Data Sheet with
some component value changes.
Feel Free to change the values back to the Data Sheet recommended
values or change to suit your circuit.

As far as I know, Pins 3 and 4 should always be shorted together.

Added are the Echo Modifications (from the Data Sheet) and
the Anti-LatchUp circuit.

The internal Input and Output OpAmps are configured as
Multi-Feedback Filters to reduce noise. 
These two OpAmpcircuits can be changed and modified as 
the user sees fit.
The other OpAmp circuits should be left unchanged.(Although, I've
seen some designs that changed the values of the Capacitors 
between pins 9-10 and 11-12 from 0.1uf to 0.47uf.

I have seen other PT2399 circuits that change the Capacitors
at Pins 7 and 8 from 0.1uf ceramic capacitors to 10uf
Electrolytic Capacitors.
I have not built a circuit with this mod, so experiment !

I've read that the Anti-Latchup circuit can be installed with
and in conjunction to the Potentiometer on Pin 6 for ajusting
the delay and not just for a Chorus Effect.
(delete R7 and connect the Collector of Q1 to Pin 6 along with
VR1 20K Speed Potentiometer).

LED1 at Pin 7 is an option that apparently prevents distortion
by limiting any overdrive signals. Recommended were Yellow or
Geen LEDs.
(apparently, it has something to do with the leds' current drive).

I've seen and heard a demo (By RRing)of a "vintage" delay circuit 
that includesa #MAX7401 8th-Order Filter IC on the output 
of the PT2399, which greatly reduced the harmonic distortion heard 
when long delay times are used.
The Data Sheet for the MAX7401 is straight-forward and should 
be easily incorportated into any PT2399 design !