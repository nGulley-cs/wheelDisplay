# wheelDisplay


Average Wheel radi of bike ~298.5mm >> Circ = 937.76540709655mm via https://www.calculator.net/circle-calculator.html  >> 36.9198979171870079 inchs == ~37 inches

Then gather RPM(rotations per minute) via 

Calculating RPM: https://endless-sphere.com/forums/viewtopic.php?t=16114

During ride, calculating RPM: Circ==Pi*((d/2)^2) | from Accelerometor get MPH {5280ft per 1 Mile} Distance=(Accel.MPH*5280)/60)

RPM = Circ/Distance


Accelerometor https://learn.adafruit.com/lsm6ds33-6-dof-imu=accelerometer-gyro 7$

RGB LED STRIP: https://www.adafruit.com/product/285?length=2 32$

RGB StripClip: https://www.adafruit.com/product/1004 2.95$

How fast LED ca be updated. https://www.pololu.com/product/2543/faqs

~ 30HZ to update all LEDs every 33ms |1000ms per 1s|

So it would work like this


Program accepts image>> maps to Hex values in grid ie 4x4

someFunc(Image>>Color grid)

then map all grid to "angle"

each angle == RGBStrip[4] =[#hex1],[hex2][hex3,[hex4] Accounting for index on one side, so picture does not appear upside down


