Steve's Christmas 2007 Freebies
===============================


While some of us have a reasonably good understanding of electronics
and have the test gear to see what's happening, I realise it must be 
frustrating for those mere mortals among you who have neither the
understanding or the oscilloscope needed to get to grips with the
workings of Serge circuits. 


Those nice people at Linear Technology have provided a rather fine
circuit simulator "LT Spice", and it's most interresting feature is
the price.  It's free!


At this price, you expect there to be a catch, and the main catch is
that the library of component models is largely stuffed with Linear
Technologies own opmps.  However, we can simulte reasonable 
approximations to several circuits, and when I find an elegant way
of adding the CA3080 and LM3900, we'll really be flying.


But for now, it is at least possible to simulate, alter and observe
the workings of a few key Serge circuits.  So, for your festive
fiddling pleasure, I have produced and tested three schematics:


Serge VCA.ASC - quarter of a 101a quad VCA

Serge WS2.ASC - Middle section of the Wave Multiplier

Serge VCFS.ASC - Variable slope VCF


All these use different opamps and transistors to the Serge originals,
but they're close enough and they work OK.  


Here's what you have to do...


Download and install LTSPice:


http://www.linear.com/designtools/software/switchercad.jsp


the models:


http://www.linear.com/designtools/software/spice_models.jsp


and the manual


http://ltspice.linear.com/software/scad3.pdf



Run the program and load any of my three schematic (.ASC) files.  

(Note that my files should be "filename.asc".  Windows has 
a nasty habit of changing them to "filename.asc.txt", so you
may have to check the extension and trim off the unwanted
".txt" part.)

Click on the running man symbol to run a simulation.


When the row of technojibber along the bottom of the page disappears,
move the mouse over the circuit and see how the cursor turns into a
scope probe or current probe.  Click, and the waveform at that point
appears in the display above.


I've set the VCA and Waveshaper to do transient analysis so you can 
look at waveforms, and I've set the CV source for the VCA to be a
sort of envelope.  The VCFS is set to do a frequency response.  


You can change the sort of test by right clicking on the bit of strange 
text at the bottom or left of each schematic.  These usually say stuff 
like:


.AC oct 3 20 20000


but a right click gets you to something less obscure.  You'll generally
want to use transient (waveform) or AC Analysis (frequency curves).


Generally right clicking on a part in before you start the simulation
lets you edit the part.  For example, changing R21 (?) the feedback 
resistor from the BP output of the VCFS back to the input opamp - will
change the resonance.  Note that you need to use "meg" not "m" of you
want to increase it to megaOhms.


(Please not that this is provided as is.  My plans for Christmas do not
include providing technical suppost for this freebie.)


Have fun



Steve - Santa mode = On 