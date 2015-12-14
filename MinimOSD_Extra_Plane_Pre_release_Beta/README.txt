Changelog
---------
R806 - 2015/12/13 - Marc MERLIN <marc_soft@merlins.org>
Rotation switching only rotates when switch changes states between low/mid/high.
This allows reusing a switch that has another function for OSD rotation.
You can rotate the OSD by flipping the switch to any other state and leaving it
there or coming back to the original location within 2 seconds.
Binary sketch size: 30,656 bytes (of a 30,720 byte maximum)


Build
-----

1) copy librariesOK/AP_Common AP_Math FastSerial GCS_MAVLink to your arduino library directory
2) get an old version of the arduino IDE (1.0.2 and 1.0.6 worked ok, 1.5.8 did not), and run 
it _after_ you've copied the libraries in the right place (arduino doesn't rescan after startup)
3) Select board Arduino Nano/ATmega328
4) build and upload


