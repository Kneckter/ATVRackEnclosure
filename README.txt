# Printable ATV Rack Enclosure
This was created with FreeCAD and I am not a CAD person, so the parts were not created in draft/draw. 
This is setup to fit 6 x96 Minis in a bay so you can fit 30 in one enclosure. 
It also has fins off the back for mounting 20-port Sipolar USB hubs without losing rack space. 2 enclosures would require 3 hubs so there are 3 fins.

This can be expanded to fit other boards if needed. Without losing comparibility for fitting the x96 Minis. All that's required are new board adaptors and to make the bay taller.

I ask that if you make useful alterations or improvements to this design, please create a pull request to share with the community.

## Parts List
 - 3D printer with filament
    - Printers and filament will vary, I'll discuss printing below.
 - 80mm x 80mm fans (No link, had these since 2005)
 - Fan screws since I ran out (https://www.amazon.com/dp/B089PX5FSZ)
 - Power adaptor for fans (https://www.amazon.com/dp/B077PW5JC3)
   - This is just an example. You need to check the power requirements of the fans. If they are 0.24v, you can power 10 fans with a 2.4v adaptor.
 - M2 x 12mm nylon standoff (https://www.amazon.com/gp/product/B08F2HLX4K)
 - M6 rack screws and cage nuts (https://www.amazon.com/dp/B09BYTWFSN)
 - 5mm x 12mm x 12mm heat sinks (https://www.amazon.com/dp/B07ZC56CRL)
   - Fits in the space left by the 12mm standoffs
 - #8-32 Threaded rod (https://www.mcmaster.com/90322A624/)
   - Only the bottom 2 rod holes need to be populated so I did not recess the top set.
   - The rods must be short enough to fit between the rack's rail mounts, which is about 450mm of 17_11/16". 
   - The hole was made to fit 5mm (0.196" or #10) rod so you can substitue for w/e the cheapest rod you can find.
 - #8-32 nuts (https://www.mcmaster.com/94450A517/)
   - Hex or square, w/e is cheapest for you. The recessed spots are setup to fit hex and should fit square.
   - The shorter the better for fitting between the rack's rail mounts.
## Printing
I printed this with a Prusa i3 MK3S+ and this is just about the max height as the print is about 203mm and the printer can go to 210mm. 
To minimize the support material, I printed these face down with supports drawn on only the fan mounts like this [screenshot]. 
I get that there are overhangs in other areas but they are not structural and I made most into bevels so they will have a little support as they print.
You can print 2 of the sections together or 1 with a couple of flat adaptors that you need to put the boards in the bays (5 sets per enclosure).

 - Print time is about 10 hours with a 0.3mm nozzel. Use a bigger one for a faster time.
 - Infill doesn't matter until the fin. I set it to 20%

## Assembly
Once you have the 3 sections and 5 sets of adaptors, you can assemble it all together.

For the enclosure, line-up the left, middle, and right sections so you can thread the rod through the 2 holes in the bottom of the sections. Put nuts on both ends and you should be good. Make sure the rod is no longer than the enclosure is wide (not included the rack mounts).

For the boards and adaptors, start with a board on top of the left adaptor and thread a standoff through the board hole into the adaptor. Then stack boards and adaptors until you have 6 boards together. Use screws for plastic to put the right adaptor on (I used the 3 screws from the ATVs for this).

## Notes
There are multiple files in this repo but only the .stl files are needed for 3D printing. The .FCStd files are the parts made in FreeCAD. Here are the names and what they contain:

 - x96_Cage.FCStd - Contains the 3 sections of the enclosure. Note that the right is a mirror of the left and the middle is a bisection of one of the left minus the rack mount.
 - x96_Flat_Left.FCStd - Contains the left side adaptor for mounting boards to. Note that it is mirrored because I didn't want to remake it.
 - x96_Flat_Right.FCStd - Contains the right side adaptor that you screw to the standoffs after putting the boards together. Note that it is mirrored because I didn't want to remake it.
<br>
 - x96_Cage_Left.stl - This is the printable left section of the enclosure. Rotate the model so the fin is in the air before printing it.
 - x96_Cage_Middle.stl - This is the printable middle section of the enclosure. Rotate the model so the fin is in the air before printing it.
 - x96_Cage_Right.stl - This is the printable right section of the enclosure. Rotate the model so the fin is in the air before printing it.
 - x96_Flat_Left.stl - This is the printable left board adaptor. Rotate the model so the bumps are in the air before printing it.
 - x96_Flat_Right.stl - This is the printable right board adaptor. Rotate the model so the recessed holes are in the air before printing it.
