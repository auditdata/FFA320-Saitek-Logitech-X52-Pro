# FFA320-Saitek-Logitech-X52-Pro for X-Plane
XMLs for adapting the X52LuaOut for use with the FF A320 Ultimate

Prerequisites

1. Download and install the excellent X52LuaOut plugin for X-Plane by Mr-Man [here](https://forums.x-plane.org/index.php?/files/file/35304-x52luaout-winmaclin/&tab=comments&page=11)

2. Confirm the default.xml provided by Mr-Man works with the stock Cessna 172 SP (Skyhawk)

3. Place the file in this repository publish.txt in the data folder of the FF A320 eg 
Desktop/X-Plane 11/Aircraft/Extra Aircraft/FlightFactor A320 ultimate/data
This exposes the internal FF A320 datarefs for AP-1, Expedite and Approach panel lights etc to illuminate joystick LEDs appropriately.

4. Move the file a320.xml from this repository which contains the absolute minimum to confirm the FFA320 and X52 are talking to each other. It should be placed in X-Plane 11\Resources\plugins\FlyWithLua\Scripts\My_x52LuaOut_definitions along with the default.xml already created by x52LuaOut. As noted in the X52LuaOut documentation you need to make sure you have an empty joystick configuration in X-plane as the a320.xml will now control the button assignments. Make sure the button assignemnts in X-plane show "Do Nothing" for Btn 0 onwards.

5. Load X-plane and choose the FF A320.

6. Confirm the MFD now shows 
"FF A320 Minimal 
Success Now try
other profiles"

7. If the MFD shows as above it is now time to remove the a320.xml file and replace it with a320full.xml and rename it a320.xml. Reload X-plane and the FFA320

8. The MFD should now show on the top line "FFA320 Ultimate" and in addition a number of the LEDs should be illuminated.


Note 1 

As mentioned in the documentation for the X52LuaOut it is possible to edit the A320.xml file and add your oun configurations.
One thing to note is the button numbers differ with X-Plane and windows combinations. In my case the button numbers are X-Plane's joystick numbers + 159. You will have to find your own button numbers. To find your own use "Plugins>FlyWithLua>FlyWithLua Macros> Show joystick button numbers".







