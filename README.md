# MonsterApocalypseRevamped (Spigot v1.14.2)

This branch is for the 1.14 version of MonsterApocalypse, I'll update this as changes differ from the 1.13 version.
And eventually, will drop support for 1.13 once the final minecraft 1.14 version is released, and stable on spigot.

# Dependencies
  All of these are optional, and MonsterApocalypse will work without them.
  
  Note: this works for spigot v1.14.1+ unless otherwise specified
    
   WorldGuard can be used to define custom flags for regions, either denying or allowing block breaking and building.
  use the flags **monsterapocalypse-destroy** and **monsterapocalypse-build** if you have WorldGuard installed.
    
   CoreProtect is used for block logging & rollbacks, you can enable the hook in the *config.yml* file.  This allows you to rollback    blocks/areas that were modified by mobs, for example, mobs placing blocks, can be rolled back using CoreProtect.
  
   ProtocolLib is just used for some QOL features, such as block breaking animations, mob animations and such.
   If there are errors on startup, make sure you install ProtobolLib before contacting me, because it's most likely just something that needed to use it.
  
  
  - **WorldGuard**  use version 7.0.0  https://dev.bukkit.org/projects/worldguard/files/2723606/download
  
  - **CoreProtect**  use version 1.17.5  https://www.spigotmc.org/resources/coreprotect.8631/download?version=276365
  
  - **ProtocolLib**  use build #425  http://ci.dmulloy2.net/job/ProtocolLib/425/
  

# Changelog
Read the full changelog here: https://github.com/FlailoftheLord/MonsterApocalypseRevamped/blob/master/MonsterApocalypseRevamped%20Changelog.md
