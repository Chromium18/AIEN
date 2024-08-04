# AIEN - AI ENhancement script
DCS World AI enhancement script for ground units

This script is possible thanks to the existance of many other scripts that I had the opportunity to use as inspiration, or partial copy, or modification due to being publicy available.
I basically leart coding starting with mist, CTLD, SLmod, dismount script, and else. All credits goes to these authors, and I am very grateful. Therefore this script is obviously public
and you should feel free to use it totally, partially or anything else for any DCS gaming purpose.

What is it?
This script is done with the purpose of rehearsing the standard DCS ground groups and units AI, 
implementing additional behaviours using the SSE, aiming to get some more dynamic and realistic
response of those units to the environment and users actions.

The script currently is focused on ground units, except SAM and medium-to-long range air defences which are not being commanded.

This works mostly by changing 2 common behaviours: 
- the fact the the units basically do not react to any hostile fire moving elsewhere: the script provide movement decision
- the fact that artillery units fire only when they directly achieve a target, which is mostly unlikely: the script provide targets on arty groups via allied units informations

It also act on another important thing on ground war: dismountable soldiers' teams. By reharsing an idea of MBot dismount script,
AIEN add soldier teams to any IFV, APC and trucks unit in the scenery. That means that a ground unit normally "unarmed" like a M-939 
might in fact transport RPG, rifle and even manpads units that will dismount from it when necessary to respond to specific menace.

In the end, if you need a specific group or more to do NOT be altered by the script, you simply have to add the exclusion tag (AIEN_xcl_tag string variable) in their group name: they will be completely ignored.


Usage informations:
- The script does not require any other script to run;
- Load the script in a "do script file" trigger after at least 3 seconds from mission start;

Notes:
- The script does not need set-up or additional coding besides the user customization variables setup below;
- It won't be properly compatible with any other script that try to change the AI behaviours for ground movers. It should be ok with IADS scripts;
- It alter the ground groups behaviour and any change will effectively "broke" any other actions given by DCS or CA user when kicking in (and that's just normal and ok).
- The script do not use any naming convention (except for the exclusion tag), it will define available AI behaviour change using DCS available parameters such as unit attributes, skills, etc.
- you will be able to customize each of its "features", by enhabling and disabling each option you want to use, here below  

Purpose and limitations:
The script does not want to provide a complete "automated ground war" thing: this is already in development by both ED and also by DSMC script by me. 
In fact, this script is a part of the DSMC script, but still usable externally as standalone
