Build
-----
1) copy librariesOK/AP_Common AP_Math FastSerial GCS_MAVLink to your
   arduino library directory
2) get an old version of the arduino IDE (1.0.2 and 1.0.6 worked ok,
   1.5.8 did not), and run it _after_ you've copied the libraries in the
   right place (arduino doesn't rescan after startup)
3) Select board Arduino Nano/ATmega328
4) build and upload


Changelog
---------
R807 - 2015/12/19 - Marc MERLIN <marc_soft@merlins.org>
--------------------------------------------------------------------------------
Previous rotation switch didn't quite work as well as I was hoping. This new
one will rotate OSD if you flip to any other position more than 200ms away from
the current one, and come back within less than 1 second.
This should work with all switches and positions and allows you to use
another switch and activate a function you don't want, but only for
a fraction for a second, come back, and generate an OSD flip in the
process.

Binary sketch size: 30,718 bytes (of a 30,720 byte maximum) (pfew :) ) 


R806 - 2015/12/13 - Marc MERLIN <marc_soft@merlins.org>
--------------------------------------------------------------------------------
Rotation switching only rotates when switch changes states between low/mid/high.
This allows reusing a switch that has another function for OSD rotation.
You can rotate the OSD by flipping the switch to any other state and leaving it
there or coming back to the original location within 2 seconds.

Binary sketch size: 30,656 bytes (of a 30,720 byte maximum)
