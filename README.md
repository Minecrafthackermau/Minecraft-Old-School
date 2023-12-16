## Minecraft Old-School

This Project is to update the old Eaglercraft 1.3_01 into something new. Welcome to Old-School!


## Compiling
(From Original Repo)

Just import this entire repository as a gradle project and use the **teavmc** gradle task. It will generate a `classes.js` in the `javascript` folder of this repository.

To change any textures and stuff, make your changes in `lwjgl-rundir/resources` and then run `epkcompiler/run.bat` to generate a new `assets.epk` in the `javascript` folder where `classes.js` is. On linux/mac, open terminal and type `chmod +x run_unix.sh` and then `./run_unix.sh` to run the tool. Copy the new `javascript/assets.epk` onto your website over the old one to update it.

**Make sure you install java and add it to your PATH, or these scripts will not work.**

To compile the server, read the [readme.txt](https://github.com/LAX1DUDE/eaglercraft-beta/blob/main/bukkit/readme.txt) in the `bukkit` folder.

**To run the desktop java runtime**, create a new java project in an IDE. Link `src/main/java` and `src/lwjgl/java` as source folders, and add all jars in the `lwjgl-rundir` folder to your build path. Create a run configuration and set the main class to `net.lax1dude.eaglercraft.MinecraftMain`, and then set the working directory to `lwjgl-rundir`. The client should then launch with no errors, if not then re-read the previous two sentances and try again.
