# The bed

Well, not the heating bed itself, which seems quite standard, but the sensors there.

# The "enhanced LeviQ 2.0"
I've done some measurings and the z-offset sensor simply is a very sensitive switch. We can probably treat it as a Z-limit switch after putting the head in the right position.
The pad next to it is a silicone pad to clean the head before testing the switch.

![A view of the Levi-Q system from above](components-above.png)

# Pinout
![A view of the heating bed from below](components-below.png)
As the pinout is quite straightforward, I won't do the fancy SVG.
* Bed and T1 are soldered directly to the board.
* Z-limit goes to CALIBRATION in motherboard. Connector: 2pin JST PH 2.0 type.
* ACC-SENSOR goes to the connector of the same name in motherboard. Connector: 7pin JST PH 2.0 type.

# The accelerometer
![The accelerometer board, taken with my microscope](acceleration-board.png)
The board contains a [LIS2DW12](lis2dw12.pdf) accelerometer; same model as in the header.
