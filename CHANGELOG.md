## TODO list
  - Put both Model and Sprite viewer.


## v0.5.0 (2006-Jan-07)
First of all thanks Zink for the help in this version and for keep it secret as I wanted :p

### Changed
  - Crop values to Info0, Info1, Info2, Info3
  - Some of the field names to be accurate.
  - Way of treat Zones. Now we only have a coordinate axis. We also have zone dimensions.

### Bug
  - Can't load a scene file when previous scene has not been found. (0000001)

### Fixed
  - Tons of things that I didn't care describing. Lots of mistakes I did in the previous versions were been fixed.

### Added
  - LBA1 life script compilation.
  - LBA1 track script compilation. (0000013)
  - Help file.
  - In-program help with content of Help file.
  - Check for new versions of the program. (0000017)
  - Window to hand choose a grid in Builder. (0000010)
  - Full compatible with Builder.
  - Feature to receive order from Builder. This two program can now work together like one.
  - Stay On Top option.
  - Batch saving feature in main menu.
  - Control Mode option for each character.
  - A "Code IntelliSense" for life and track script. If you press CTRL+Space will be popup a list with all commands available for that script. This will be an extra help when you start coding and doesn't remember the commands.
  - Number of current line and current column for each script.


## v0.04 (release 6) (2006-Feb-13)
  - **[Changed]:** Program name to LBA Story Coder. Now with this name we can automaticly know what this program could do ;)
  - **[Changed]:** Now working with both Binary and Text mode formats. You can also set this program in LBA Package Editor tool for scene files.
  - **[Changed]:** Scene file types according with LBA Package Editor.
  - **[Changed]:** Actors/Zones/Tracks X,Y,Z coordinates edits. Now we can put the right coordinates according with the grids. Anyway the scrolls are there for a fast change, but I suggest to use the edits. For example each layer in LBArchitech increase 256 in Y position. That way you can easly set a new coordination for your actor/zone/track. Also added feature to disabled this.
  - **[Changed]:** Actor display in a new window. This time only image of actors are displayed. Future versions will have the 3D model viewer compatible.
  - **[Enabled]:** Zones and Tracks again. Now fully compatible.
  - **[Enabled]:** "Is sprite actor" check box under Actor Static Parameters window because the creation of new actors in scenes.
  - **[Added]:** Compitble for LBA2 scenes. You can now also edit some of the scene definitions. Note that this are yet in tests and isn't all compatible.
  - **[Added]:** New file type, LBA Story Coder Project (*.scp), to save parameters according with the script. This will save all scene content in a special format where we'll have also the script comments that will not be under the binary/text exported scenes.
  - **[Added]:** Association file type for all compatible files (*.scp, *.ls1, *.ls2 and *.sce)
  - **[Added]:** New option under Zones tabs where we could set diferent types of Zones. Only for LBA1 scenes for now.
  - **[Added]:** Completely actor script decode with indent.
  - **[Added]:** New option to display actor scripts with syntax hightligh. (Experimental) (can slow a bit script load, you need to wait 1/2 seconds :/)
  - **[Added]:** New window with script help. Now you can see what you exactly are doing in the script. Note that this is only available for LBA1 scenes.
  - **[Added]:** New options under atmosphere tab where we could see some scene enviroment options (Experimental because I need to know first what they are exactly).
  - **[Added]:** Lots of new options under Settings menu.
  - **[Added]:** Feature to read content of File3D.HQR file for restringe body/anim entities for each actor. This only work for now with LBA1 scenes. When LBA2 will be more compatible I'll do such thing since isn't so diferent.
  - **[Added]:** Feature to open the grid related with the opened scene. Note that the file name must have the scene number before the scene name like LBAPackEd did (e.g. scene001_something or 001_something). (Experimental)
  - **[Added]:** Also added feature to manipulate Tracks, Zones and Actors under LBArchitect. (Experimental)
  - **[Added]:** Comentary character for script code. Use 'REM' when you want to make a comentary under the script code in a new line.
  - RIGHT example:
```
		REM first commentary
		LABEL 1
		ANIM 5
		REM second commentary
		STOP
		END
```
  - WRONG example: (not supported in this version)
```
		LABEL 1 REM first commentary
		ANIM 5
		STOP REM second commentary
		END
```
 - **[Fixed]:** Actor and static parameter windows when we close a scene inside the program. (They were always opened)
 - **[Fixed]:** Bugs in Actor, Tracks and Zones New, Clone and Remove options. This is also now compatible with LBArchitect.
 - **[Fixed]:** Bugs in binary save routines. The binary mode isn't all yet compatible since the scripts aren't yet compiled. I'm still working on it, so be pacience please :)


## v0.03 (2004-Dec-31)
 - **[Fixed]:** Incorrectly actor position disaplay
 - **[Fixed]:** Incorrectly talk color saved.
 - **[Enabled]:** Button to close the current file.


## v0.02 (2004-Dec-31)
  - This version is to edit only the dumped scenes, included with this program and with TwinEngine. The disabled options will be available in the next release. I'm release this for people try to make something with life and move script, creating new actors and so on...
  - **[Added]:** A new window with the static value parameters.
  - **[Added]:** A new window with to edit the Actor Script (Life and Move Script).
  - **[Added]:** Creatiation of new actors.
  - **[Added]:** Clone and Remove actors.
  - **[Added]:** Dragged file option. Now you can drag scene files in the window ;)
  - **[Added]:** Original LBA main pallete to the Actor Talk Color. (thanks to Zink for helping me)
  - **[Added]:** Bonus type Combo-box. Now you can directly choose the bonus type. (Zink ideia)
  - **[Added]:** Change actor position with the mouse. This thing ins't working perfect because works like the scroll. (Zink ideia)
  - **[Added]:** Text bank combo-box with the islands names. You now can choose the texk bank according with the island.
  - **[Fixed]:** Bug in the Actor Angle thing.
  - **[Fixed]:** Rotation Speed bar. Now 100% is fast and 0% is slow.
  - **[Fixed]:** Language bugs (thansk to Zink).
  - **[Disabled]:** Feature to open the scene high quality resource directly.
  - **[Disabled]:** Settings menu.
  - **[Disabled]:** View dumped scene menu to view the scene file in text mode. This feature is compatible with TwinEngine dumped scenes.
  - **[Disabled]:** Save Message Dialog when you close the program with an edited file.
  - **[Disabled]:** Recognized Invisible Actors (Telepod Actors and Meca-Pinguins).
  - **[Disabled]:** Zones and Tracks display.
  - [Fixed/Disabled] Incorrectly file save. The saved file loose some actors and sometimes crashed the game.


## v0.01b beta (2004-Aug-14)
   - **[Fixed]:** Bug in "Save as" option. (thanks to NightShadow)


## v0.01a beta (2004-Aug-13):
  - **[Added]:** "Save as" option.
  - **[Added]:** "Armure" to "Armour", "Speed" to "Rotation Speed" and "Behavior" to "Mode".
