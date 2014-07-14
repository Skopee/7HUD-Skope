====
7HUD-Skope
====
To install:

	- Download via the "Download ZIP" button on the right side of the github page. 
	- Extract to your Steam\Steamapps\common\TeamFortress2\tf\customize

To uninstall:

	Delete the folder.

CUSTOMIZING
------------------------------------------------------
------------------------------------------------------

FOG'S CROSSHAIRS:
	
	- To enable Fog's Crosshairs, navigate to your hudlayout.res file, found in the scripts folder. Change the "enabled" value under the Fog's Crosshairs heading to "1". Then pick your Crosshair using the included list of crosshairs and insert the character of the crosshair in the "labeltext" line.
	- To enable a crosshair flash when you hit a player, find HudAnimations_tf.txt in the scripts folder and under the first heading, DamagedPlayer, there will be instructions.

------------------------------------------------------

Normal CROSSHAIRS

Activate the crosshair by going to your scripts folder and then hudlayout.

Change visible from 0 to 1.

	If the crosshair isn’t centralized do the following:

	1. Go to your scripts folder and then hudlayout.
	2. Change the xpos and ypos values. (xpos is for horizontal and ypos is for vertical).
	3. Start TF2 and see if it’s centralized.
	4. If not, Alt+TAB and try another value. 
	Go back into the game and type hud_reloadscheme in console.
	5. Do this until you’re happy.

	If you want to change the crosshair size go to your resource folder and then CLIENTSCHEME. 
	Change the tall value to whatever you like.
	
	If you want to change the colour go to your scripts folder and then hudlayout. 
	Change the fgcolor to the colour you want. 
	If you don't know how to customize colors go to the CLIENTSCHEME file in /resource/.
	You can find information there.
	Example: "fgcolor"  "255 0 0 255" would make the crosshair red.

	(If the crosshairs isn’t centralized then you sometimes have to change “wide” and “tall” too, not just “xpos” and “ypos”)
	
	(Some CrossHairs are combinations, you need to activate more than one)

CHAT BOX:

	Rename the appropriate BaseChat.res file located in your resource/ui folder to "BaseChat.res". For example, I want my chat box in the bottom left corner. I would rename "BaseChat - BOTTOM.res" to "BaseChat.res" and vice versa.

------------------------------------------------------

SCOREBOARD:

	To change scoreboard to 6v6, simply hit click the "Scoreboard" button on the main menu or the in-game menu.
	
	To change the scoreboard to the old one, simply delete Scoreboard.res, and rename Scoreboard -OLD.res as Scoreboard.res

------------------------------------------------------

KILLFEED:

	To increase line spacing:
	
		1. Go to /scripts and then "hudlayout.res"
		2. Search for "DeathNotice" (ctrl+F)
		3. Increase the value for "LineSpacing"
			The higher the value the bigger the distance between entries in the Killfeed
		3: Save
	
	To increase size:
	
		1. Go to /scripts and then "hudlayout.res"
		2. Search for DeathNotice" (ctrl+F)
		3. Change the number in the "font" value to 9, 10, or 11.
		4. Change the "LineHeight" value in accordance with your new font number. 
			- i.e. font: Regular10. LineHeight: 10.

You can enable a background for the KILLFEED in the CLIENTSCHEME 

------------------------------------------------------
------------------------------------------------------
PERSONAL TROUBLESHOOTING
------------------------------------------------------
------------------------------------------------------

SCOREBOARD PING CLIPPING:

	1. Navigate to ScoreBoard.res in your resource/ui folder
	2. Under the first heading (scores), find "ping_width".
	3. Lower the value, maybe 3-4 down, save the file, alt-tab into the game if it's open and put "hud_reloadscheme" into the console. This refreshes all the .res files in your 7HUD folder. If you're not in-game, simply launch TF2
	4. You can also change the "name_width" and/or "score_width" values I move it over more all-togetherly


------------------------------------------------------
------------------------------------------------------
RECOMMENDED OPTIONS
------------------------------------------------------
------------------------------------------------------

CHANGE NET_GRAPH SIZE IF YOU USE IT:

If you use net_graph to monitor FPS/ping/lerp etc., I recommend changing the net_graph to a smaller size

	1. Put these in your console for best results:
	2. net_graph 1
	3. net_graphproportionalfont 0
	4. net_graphheight 48
	5. net_graphpos 1

------------------------------------------------------

BIND 2 FAVORITE SERVERS TO MENU BUTTONS:

	1. Put these codes in your autoexec.cfg:
	2. alias Server1 "connect <ip here>"
	3. alias Server2 "connect <ip here>"
	4. Server1 corresponds to the top right button, Server2 the bottom. 
	

------------------------------------------------------

ENABLE CLOSED CAPTIONS:

	1. Put “closecaption 1” and "cc_predisplay_time 0" in your autoexec.cfg.
