Autopilot ( FILTERSCRIPT! )
Requirements:
-ZCMD
-RouteConnector aka GPS Plugin
-Server version >= 0.3a

The Script has 3 defines which you can use:
#define USE_TIMERS
#define DEPRECATE_Z
#define USE_SMOOTH_TURNS --- thanks to richardcor91

the USE_TIMERS define will force the script to use timers instead onplayerupdate.
the DEPRECATE_Z define will keep your vehicle Z velocity, else if not defined the 
destination Z velocity will be calculated and set to the vehicle.
the USE_SMOOTH_TURNS will turn the car very smoothly at turns.

Please take a look in the script at :
{{{new places[PLACES][location]}}}


You will se all location names, then the X Y Z coords.

The main command is /autopilot (or /ap),
the available syntaxes are:
/ap 0.xx (eg: /ap 0.55) - set the speed of the autopilot (the speed of the car...).
/ap <destination name> (eg /ap LS-a will drive you to the los santos airport) - the destination the autopilot should drive you to.
/ap stop - will stop the autopilot.

The other command is /interval , this is the command is only available when you have
USE_TIMERS defined. This will set the amount of miliseconds between each call.

Please note this filterscript is not supposed to be used on servers with many players, or at least limit the usage to ~ 5 players max.

A video can be found here:
http://www.youtube.com/watch?v=EHj7GavsbqQ

download:
http://gpb.googlecode.com/files/AutoPilotV0.1.zip
