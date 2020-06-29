### Recipe Database

|   | Size | Health | Power | Research Prerequisites | Resource Cost |
| - | ---- | ------ | ------------- | ---------------------- | ------------- |
| <img src="https://github.com/zymex22/Project-RimFactory-Revived/blob/master/Textures/SAL3/DISK_HARDWARE4_north.png?raw=true" width="32" height="32" /> | 1x1 | 150HP | 250W | Magnetic Tape | 1x <a href="https://github.com/zymex22/Project-RimFactory-Revived/wiki/Construction-and-Crafting-Resources#machine-frame"><img src="https://github.com/zymex22/Project-RimFactory-Revived/raw/master/Textures/Common/MachineFrame.png?raw=true" width="16" /></a><br />20x <a href="https://rimworldwiki.com/wiki/Steel"><img src="https://rimworldwiki.com/images/c/c9/Steel.png" width="16" /></a><br />1x <a href="https://rimworldwiki.com/wiki/Component"><img src="https://rimworldwiki.com/images/4/40/Component.png" width="16" /></a><br />1x <a href="https://github.com/zymex22/Project-RimFactory-Revived/wiki/Construction-and-Crafting-Resources#recipe-data-disk"><img src="https://github.com/zymex22/Project-RimFactory-Revived/raw/master/Textures/SAL3/datadisk.png?raw=true" width="16" /></a> |

The Portable Recipe Database can import recipes from nearby worktables. Afterwards, when reinstalled near assembler(s), it will upload its recipes to them.<br /><br />Blue cells are import range for the database.<br /><br />Uploaded recipes and bills will be lost if the database is moved or destroyed.<br /><br />I wonder what all these other buttons do...

### Assembler

|   | Size | Health | Power | Research Prerequisites | Resource Cost |
| - | ---- | ------ | ------------- | ---------------------- | ------------- |
| <img src="https://github.com/zymex22/Project-RimFactory-Revived/blob/master/Textures/SAL3/smart_assembler.png?raw=true" width="96" height="96" /> | 3x3 | 250HP | 625W | Universal Autocrafting | 2x <a href="https://github.com/zymex22/Project-RimFactory-Revived/wiki/Construction-and-Crafting-Resources#robotic-arm"><img src="https://github.com/zymex22/Project-RimFactory-Revived/raw/master/Textures/Common/RoboticArm.png?raw=true" width="16" /></a><br />1x <a href="https://github.com/zymex22/Project-RimFactory-Revived/wiki/Construction-and-Crafting-Resources#machine-frame"><img src="https://github.com/zymex22/Project-RimFactory-Revived/raw/master/Textures/Common/MachineFrame.png?raw=true" width="16" /></a><br />120x <a href="https://rimworldwiki.com/wiki/Steel"><img src="https://rimworldwiki.com/images/c/c9/Steel.png" width="16" /></a><br />10x <a href="https://rimworldwiki.com/wiki/Plasteel"><img src="https://rimworldwiki.com/images/c/c5/Plasteel.png" width="16" /></a> |

An automatic assembler controlled by a computer. Despite being called an assembler, it's also capable of simpler procedures such as cutting stone blocks, and refinery work.<br /><br />Downloads recipes from an adjacent recipe database.<br /><br />White cell is input range, Blue cell are db range, Yellow cell is output

### Adaptive Assembler

|   | Size | Health | Power | Research Prerequisites | Resource Cost |
| - | ---- | ------ | ------------- | ---------------------- | ------------- |
| <img src="https://github.com/zymex22/Project-RimFactory-Revived/blob/master/Textures/SAL3/correcting_assembler.png?raw=true" width="96" height="96" /> | 3x3 | 350HP | 700W | Self Correcting Assemblers | 2x <a href="https://github.com/zymex22/Project-RimFactory-Revived/wiki/Construction-and-Crafting-Resources#robotic-arm"><img src="https://github.com/zymex22/Project-RimFactory-Revived/raw/master/Textures/Common/RoboticArm.png?raw=true" width="16" /></a><br />1x <a href="https://github.com/zymex22/Project-RimFactory-Revived/wiki/Construction-and-Crafting-Resources#weak-ai-chip"><img src="https://github.com/zymex22/Project-RimFactory-Revived/raw/master/Textures/Common/WeakAICore.png?raw=true" width="16" /></a><br />1x <a href="https://github.com/zymex22/Project-RimFactory-Revived/wiki/Construction-and-Crafting-Resources#adv-machine-frame"><img src="https://github.com/zymex22/Project-RimFactory-Revived/raw/master/Textures/Common/MachineFrameLarge.png?raw=true" width="16" /></a><br />10x <a href="https://rimworldwiki.com/wiki/Plasteel"><img src="https://rimworldwiki.com/images/c/c5/Plasteel.png" width="16" /></a><br />150x <a href="https://rimworldwiki.com/wiki/Steel"><img src="https://rimworldwiki.com/images/c/c9/Steel.png" width="16" /></a><br />2x <a href="https://rimworldwiki.com/wiki/Component"><img src="https://rimworldwiki.com/images/4/40/Component.png" width="16" /></a> |

An automatic assembler controlled by a primitive AI.<br /><br />The simple artificial neural network enables it to learn; to be more precise and efficient at individual recipes. Slowly overwrites currently unused recipe algorithms, as it has limited processing and memory capacity.<br /><br />Downloads recipes from an adjacent recipe database.<br /><br />White cell is input range, Blue cell are db range, Yellow cell is output

***

### Assembler / Recipe Database Usage
Once you have built, for example, a Machining Table; build or place a Recipe database adjacent to the table. Once built or placed, click on the Recipe database and observe the "Import recipe" action. Clicking that will open a contextual menu showing you the recipes available in the Machining Table. Clicking on any of those recipes will begin the importing process, that process will  take time.

Once you have imported one or more recipes into the Recipe database, you can place it adjacent to either an Assembler or Adaptive assembler. This, in turn, will allow the adjacent  assembler(s) to use the recipes from the Recipe database to setup bills as if it were the initial Machining table.