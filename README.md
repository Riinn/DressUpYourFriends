# DressUpYourFriends
Version 0.1: Initial release with basic working features

A Tera Proxy Module to change the look of your friends, enemies or anyone in your visible vicnity. Appearance is Client Sided!!! Using the commands on anyone will cause their equipped costumes/equipment to change to look like yours. Currently copies every costume/equipment on you, but appearance (skintone,hair,face etc) is unaffected.

Might cause some lags in heavily populated areas? I dont know. But you can just disable the module and this clears all entry and effectively prevents the logging of targets.

Yes i know the code is messy af with comments everywhere. Just don't look LUL, i'm new to JS. Feel free to share, this is harmless, but risk is on you since you are using a proxy anyway.

## General instructions
When logging in you should see a message 'current equipped saved'. When you change your appearance in any way (except using proxy modules), you should see this message again. This signifies the current equip you have is saved and to be copied onto your targets.

To reset a target's appearance to their original, just move out till you cannot see them and move back in to reload. I miggghhhhhht add a function in the future but i dont see why this is important because doing that will require the saving of all character's apearances, much easier to just move back and in right?

Defaults: Module is enabled, Maintain appearances thorugh target changes enabled.
## Commands:
- !dressup (name): Dress up the named person to look like you. Can be in any captialization, just spelling matters. Eg: '!dressup seren' can dress up any igns seren,Seren, SEREN, seReN,etc. 
- !du maintain: Toggles whether to maintain the changed costume on others even if they change their look.-Untested fully yet
- !du: Toggle enabling/disabling of module. Disable module will disable logging of targets around you, disables saving of your appearances and clears all saved targets. This effectively makes the module disabled. You have to unequip and re-equip something to save your appearances (look for the message that indicates this), as well as move out and back into the visible vicinity of your targets to save their ids after re-enabling the module.
- !du(number): change modes. Not Implemented Yet.

## Known bugs
- It will not work for targets of different Race. Although it seems to work well regardless of classes.
- Also does not seem to work for targets of different height/thigh/shape whatever when it comes to costume, though it worked alright when i unequipped costume and left the equipments or inners(fml,see safety advice 1) equipped. (Investigate this soon, prob one of the unk values), so only costume is affected by shape differences. 
- Attempting to do those above will cause a floating head effect. Simply move out and back from the sight of the target to reload their appearances. It can actually work sometimes, i tested on a castanic and lul, have you seen a elin using arccannon before?
- Probably will not save module-changed appearances by other modules yet. Will try to do that next, after working out the costume issues.

## Safety advice
- Forced erp is a henious crime in the land of baldera. I am not responsible should you be caught by the popo(ri) due to misuse.
- It is impossible for me to test every aspect so expect bugs here and there.


## TODO
- Allow changing of appearance via greeting the target. (So you dont have to type any names :) )
- Making costume work regardless of shape.
- Save player equipments from other modules that changes looks too (filter.fake=true)
- Give a command to allow players to customize their saved look using item ids, so they can put different costumes on the changed target and do not necessary become a copy of the target costume. Especially weapons, which should not be replaced. No more Elin carrying an arcannon. That looked so weird. 
- Give different options to users that allow them to only copy certain equipments. (ie: only change body costume, while leaving the rest as target's original costume)- requires indexing 
