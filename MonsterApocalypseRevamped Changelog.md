Henlo, i'll be posting all the updates and changes here as i progress with the recode of the plugin!
Check back for further updates :p

Estimated Completion: 60%

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


(Feb-24-2019)
 - Made block attacking more realistic, mobs won't keep breaking blocks that they can't see, and will tend to break block at eye level or that are in between then and the player they're targetting.
 - Actually fixed per-world-settings, they should work just fine now.
 When a new world is created, the plugin will add it to the blacklist in the 'GeneralSettings.yml' file.
 That forces MosnterApocalypse to disable mob features in that world. To enable them simply remove the world from the 'DisabledWorlds' section in the **GeneralSettings** file.
 
 I removed alot of uneccessary settings from the files, and changed up some of the formatting, so for the next release, you'll need to delete your old files again. It's going to happen a ton, as i keep changing the format of the files/ how the settings are read & setup.

(March-3-2019)
  - Block breaking will now have a few seconds of delay before the mobs break them. I will try and get some fancy break animations working. (If ProtocolLib is installed) hopefully next update.
  
(March-10-2019)
  Sorry for dragging out the updates again...
  - Block placing is coming along nicely, the mobs will attempt to build up untill they reach eye level with you, at which point, they'll either fall down and build back up again, or  get frustrated and start breaking blocks.
  I will release another build on the eleventh.
  
(March-16-2019)
  - Began work on mob drop customization.
  
(March-17-2019)
  - Ability to set drops for mob deaths added, working on support for custom items.
  
  I will release a sixth build once i have fully tested the mob-drops settings.
  Be sure to check for it within the next couple of days!
 
(March-21-2019)
  - Wrapping up Mob drops.
  I should have the next build out by March 22nd
  
(March-26-2019)
  - Mob drops are 100% functional.
  Featuring a fully customizable item drop support, as well as options for amount and chance.
  
  To manually add custom items, (like items from another plugin) simply type **/ma editdrops <mob-name>**
  It will open a GUI where you can put any items in that you want, any existing Custom drops for that mob will be shown in the gui, and you can manually edit them from there.
  Items are saved automatically once you close the GUI.
  There is a chance option in each mob's settings file labaled *'CustomItemDropChance'*
  This means that it will randomly pick **one** item out of the list and add it to the mob's drops using that percentage chance.
  I will try and add unique chances for each custom item soon. But this system will have to suffice for now.
  
  You can also add custom drops the normal way, under the *'Drops'* section, just add the block name you want and optionally the amount and percentage chance to drop.
  Follow this format:
  ```
    Drops:
    - cobblestone:1:75
    - dirt:3
    - bread:5:23
    - stone_shovel
  ```
  This means that it will drop 1 cobblestone with a 75% chance, 3 dirt with a 100% chance, 5 bread at 23% chance, and one stone shovel (100% chance)
  the format being: `- <item>:<amount>:<chance>`
  I will release a seventh build alongside this.
  
(April-1-2019)
  Added tab-completion & changed up some commands.
  
(April-9-2019)
  Added WorldGuard support (make sure you're using the latest v7.0.0 worldguard for 1.13+)
  There are two custom flags for now, which you can add to regions.
    **monster-apocalypse-build** and **monster-apocalypse-destroy** If set to 'deny' in a region, will prevent mobs from breaking/placing blocks in that region.
  I will eventually add a-lot more flags which you can use to customize what mobs can do, such as entering a region, spawning in a region & more.
  Again, more on that later :D
  
  Released an eighth build with this update also.
  
(April-11-2019) 
  Working on advanced block placement. This will include stairs, bridges and walls.
  ... more on this later ;P
  
(May-14-2019)
  Picking back up on complex block placement.
  It's been a while! 
  
(May-15-2019)
  Added block decaying, blocks placed by mobs will decay after a certain amount of time.
  
  **WARNING** If you reload MonsterApocalypse, or restart the server, any placed blocks WILL NOT decay. 
  Instead, if you have CoreProtect installed, use `/co rollback r:<radius> t:<time>` and it will restore all block placements to their previous state.
  settings are in the `GeneralSettings.yml` file under **BlockBuilding -> BlockDecay & BlockDecayTime** the Block decay time is in *seconds*.
  
  I'll be releasing the ninth build today as well ;)
  
  Again, if you find any issues with this build, please let me know on discord!
  
