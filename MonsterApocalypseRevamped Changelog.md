Henlo, i'll be posting all the updates and changes here as i progress with the recode of the plugin!
Check back for further updates :p

Estimated Completion: 40%

(Jan-17-2019) Finished Spawnpoints Command Tutorial

(Jan-18-2019) 
- Wrapping up Spawnpoint Commands, working on FileLoader methods, saving configurations, and loading settings.

(Jan-19-2019) 
- Beginning work on auto-spawning based on the spawnpoints. Smoothed out the spawnpoint editor.

(Jan-20-2019) 
- Spawnpoints' auto-spawning finished, adding more options and args to the spawnpoint command...

(Jan-21-2019) 
- Plugin loads default values into the MobSettings.yml file...
- Added controls and toggles for Natural Spawns... (more on that later)

(Jan-22-2019)
- Starting work on Mobs' AI.
this will be the starting point for forced mob-aggro, air-bridging to players, 
climbing/building over walls and obstacles... and loads more!

(Jan-23-2019)
- Distinguishes between Hostile, Passive, and non-AI mobs.
- Adding distinctive behaviors for each type.
- made file handler save files on shutdown...
- when plugin loads, it checks if the server is running Spigot v1.13...
if not, it shuts down the plugin with an error message.

(Jan-24-2019)
- Mobs will now auto attack if you get within their range.
- added toggle for MegaAggro and variables to control how far away the mobs will get aggro'd at you.
- speed modifiers added.

(Jan-31-2019)  
- redoing the file loading methods... the settings file isn't modifiable from the server end.
- adding wall-attacking/block breaking, range for mobs.
A whitelist of mobs who are allowed to break blocks, and a list of blocks that mobs can break.

(Feb-1-2019)
- made a ton of progress on the wall attacking methods... 
- released another experimental build on GitHub.

(Feb-11-2019)
- Finished up wall attacking, it looks completely realistic now!
- Beginning work on entity target AI, the abilty for any mob to shoot a player with a custom projectile... 
And also passive mobs will be able to attack players as well... 
This is going to take a TON of work, so don't be surprised if i don't show any progress reports for the next week or so.
- Finally, i'll release a third build, which boasts the finalized wall attacking methods. :)
Again, thanks for y'alls patience, i'm struggling to keep up with a number of different projects on top of this one.

(Feb-13-2019) 
- working on jump methods for zombie bridging/building.
- added sounds to block breaking, suggestion from @kuncroft

(Feb-19-2019)
 Sorry for the long delay in updates, i had some other plugins i was working on, i'm going to be pushing alot on this one now.
 So expect to see alot of updates within the next week!\
 
- Added Per world settings. These are exactly the same as the contents of the 'GeneralSettings.yml' file. So just copy paste!
The world config files will be loaded up on startup, and they will contain a copy 
of your current 'GeneralSettings.yml' file if you created a new world or haven't configured that world yet.
- Still working on block building, i have some plans in progress, which will be out in the next couple of releases, these will include
features such as wall building, stairs, bridging across gaps, placing lava on players, shooting arrows, trapping players in cobwebs...
and alot more that i may or may not have planned yet, feel free to give me more suggestions via discord!  :>
- Will release a fourth build with this update too, just so y'all can try out the new world settings ;p




