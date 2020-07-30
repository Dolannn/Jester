# Jester Mission Making Guide

Author Dolan:

First thing's first, load 3den Enhanced (https://steamcommunity.com/workshop/filedetails/?id=623475643), launch arma and open the editor. 

Save your mission right away, and make sure "Binarize the Scenario File" is not ticked, this will come in handy if you're building a mission and we remove a mod, or if you accidentally load something like JSRS which creates a required addon automatically despite being client side. After you've saved, open your mission, click "Scenario > Open Scenario Folder" and drag the following .sqf files to it:

initPlayerLocal.sqf

initServer.sqf

onPlayerRespawn.sqf



Next hit "Attributes > Multiplayer", do the following steps

Untick Enable AI

Change Respawn from "Disabled" to Respawn on Custom Position, then untick everything in the "Rulesets" box

Untick "Show Scoreboard"

Tick "Allow Manual Respawn" 

Hit OK

Add a mapmarker via going to the upper right side of your screen in the editor and hitting the market button, or hit F6.

Pick a marker, place it where you'd like players to respawn, then double click the placed marker and change the "Variable Name" to one of the following:

respawn_west

respawn_east

respawn_guerrila

respawn_civilian

If we're playing as BLUFOR, make the variable marker "respawn_west" ... If we're playing as OPFOR, make the variable marker "respawn_east" ... If we're playing as GREENFOR/INDFOR, make the variable marker "respawn_guerrila" ...  and if you're a weirdo and we're playing as civies, make it "respawn_civilian".

IF you don't want this marker to be visible, just change the "Alpha" to 0%.

Place a playable unit, this will be you! If we're playing as BLUFOR, make sure to not place a BLUFOR RHS unit, their vests are too strong and tanky (if you're unsure if you've placed one, hover your mouse over him and see if his classname has "rhs" at the start of it. Alternatively right click on the unit and check his vest, change it to a CUP vest.) Once you've checked that double click on your unit! Give him a variable name (I'll be calling mine "God"). Whilst we're here make sure he's playable and set as the player, below that change your role description to "Zeus@Crossroads" without the quotation marks. This means that in the slot up screen your callsign will be "Crossroads" and role will be "Zeus". Scroll down to "Object ACE Options", open it up and set the unit as a Regular Medic. This allows us to transfuse blood. Hit Okay.

Next Click on the BlueBox (will be Red if you placed OPFOR, Green for Independent etc) above the unit you just placed, changed the "Callsign" to "Crossroads", this means when we're playing the mission, we can see where the Callsign is on the map. Since you're Zeus you might not want to be seen on the map at all, if so scroll down to "Composition: ACE Options" and Tick "Disable BFT", hit Okay.

We're finally going to give your own player slot Zeus. Hit F5 or go to "Modules > Zeus > Game Master" place it on the map and double click the module. Remeber what you set your player's variable name to? I put mine as "God" so I'm going to type it into the Owner tab, whilst you're here change the "Defualt addons" to "All addons (including unofficial ones)", then hit Okay.

Right click on yourself, give yourself atleast an AN/PRC-152 via right clicking yourself and opening the ACE Arsenal.

Now place your friendly Jester Units, set them as "playable", remember to scroll down to "Object ACE Options", open it up and set the units as a Regular Medic. From there sort their gear out, remember things such as giving a 152 to Team Leaders and Fire Team Leaders, about 12 Elastic Bandages for each player about 2x Tourniquets, about 2x Morphine, about 2x Epi, about 6 Mags, NV Goggles (Wide) if you're using NVG's etc etc, Medics will need a PAK / Personal Aid Kit and a good few thousand mL's of blood. Remember to set their Role Description via this template (don't include the quote marks again): "InsertRoleHere@InsertCallsignHere" and click the blue box above the Unit and type the appropriate callsign.

Thats all for the bare basics, included is a .pbo with everything we just did, feel free to de-pbo it with pbo manager (found here: https://www.armaholic.com/page.php?id=16369), place this file into C:\Users\yournamehere\Documents\Arma 3 - Other Profiles\yournamehere\mpmissions, once it's in that directory, right click the .pbo > extract to JesterMission_TemplateVR. You'll be able to open it up in the Arma Editor now, and copy paste everything into a map of your choice.

JesterMission_Template.pbo can be found attached to this folder.
