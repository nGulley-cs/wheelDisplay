# wheelDisplay


Average Wheel radi of bike ~298.5mm >> Circ = 937.76540709655 via https://www.calculator.net/circle-calculator.html

Then gather RPM(rotations per minute) via 





How fast LED ca be updated. https://www.pololu.com/product/2543/faqs

~ 30HZ to update all LEDs every 33ms |1000ms per 1s|

So it would work like this


Program accepts image>> maps to Hex values in grid ie 4x4

someFunc(Image>>Color grid)

then map all grid to "angle"

each angle == RGBStrip[4] =[#hex1],[hex2][hex3,[hex4] Accounting for index on one side, so picture does not appear upside down.
