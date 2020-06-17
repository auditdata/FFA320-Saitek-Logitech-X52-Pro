# FFA320-Saitek-Logitech-X52-Pro for X-Plane
XMLs for adapting the X52LuaOut for use with the FF A320 Ultimate

Prerequisites

1. Download and install the excellent X52LuaOut plugin for X-Plane by Mr-Man [here](https://forums.x-plane.org/index.php?/files/file/35304-x52luaout-winmaclin/&tab=comments&page=11)

2. Confirm the default.xml provided by Mr-Man works with the stock Cessna 172 SP (Skyhawk)

3. Place the file in this repository publish.txt in the data folder of the FF A320 eg 
Desktop/X-Plane 11/Aircraft/Extra Aircraft/FlightFactor A320 ultimate/data
This exposes the internal FF A320 datarefs for AP-1, Expedite and Approach panel lights to illuminate joystick LEDs appropriately.

4. Move the file a320.xml from this repository which contains the absolute minimum to confirm the FFA320 and X52 are talking to each other. 

5. Load X-plane and choose the FF A320. When it has completed loading the MFD may show an error or may not. If it does the reason is the A320 datarefs are not available when FlywithLua loads the script. To get around this, once the A320 is loaded go to the menu item "Plugins>FlyWithLua>Reload all Lua script files" This will then clear the failed to load error.

6. Confirm the MFD now shows 
FF A320 Minimal 
Success Now try
other profiles

7. If the MFD shows as above it is now time to remove the a320.xml file and replace it with a320full.xml and rename it a320.xml. There is no need to reload the A320 but you now need to reload the X52LuaOut script. This is done by going to the menu item "Plugins>FlyWithLua>Reload all Lua script files". Each time you reload the A320 you will need to reload the Lua script files. The x52LuaOut developer has told me this could be fixed in the next version.

8. The MFD should now show on the top line "FFA320 Ultimate" and in addition a number of the LEDs should be illuminated.


Note 1 

As mentioned in the documentation for the X52LuaOut it is possible to edit the A320.xml file and add your oun configurations.
One thing to note is the button numbers differ with X-Plane and windows combinations. In my case the button numbers are X-Plane's joystick numbers + 159. You will have to find your own button numbers. To find your own use "Plugins>FlyWithLua>FlyWithLua Macros> Show joystick button numbers".


Note 2

The assignment of buttons for commands "a320/Panel/FCU_SpeedMode_switch_pull"  and command "a320/Panel/FCU_SpeedMode_switch_push" seem to crash the A320 Speed mode system. I have no idea why! I have commented them out in the script. Other similar commands work perfectly. The workaround it to assign them by the X-plane Joystick system. These are the only commands assigned to buttons in the X-plane joystick system all others are assigned in the X52LuaOut script.





