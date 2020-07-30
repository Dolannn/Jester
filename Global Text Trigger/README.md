# Jester SQF Tuts\Global Text Trigger
Author: Dolan
Place a trigger via pressing the flag icon near the upper right side of your screen or by pressing F3, click any of the triggers.
Double click the trigger you just placed, in the trigger transformation tab, change the size of the trigger to what you desire.
Set the Activation to "Any Player" (you can use any type you want, but for simplicity lets go with this one)
Click "On Activation", then copy and past this template and edit it as you need to.

any=[ 
 [ 
  ["insert mission name here","<t align = 'center' size = '0.7'>%1</t><br/>"], 
  ["insert date here","<t align = 'center' size = '0.7'>%1</t><br/>"], 
  ["insert remark here","<t align = 'center' size = '0.7'>%1</t>"] 
 
 ] 
] spawn BIS_fnc_typeText;