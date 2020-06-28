### Recipe Database

|   | Size | Health | Power | Research Prerequisites | Resource Cost |
| - | ---- | ------ | ----- | ---------------------- | ------------- |
| <img src="https://github.com/zymex22/Project-RimFactory-Revived/blob/master/Textures/SAL3/DISK_HARDWARE4_north.png?raw=true" width="32" height="32" /> | 1x1 | 150HP | 250W | Magnetic Tape | 1x PRF Machine Frame<br />20x Steel<br />1x Component Industrial<br />1x Rim Factory Data Disk |

The Portable Recipe Database can import recipes from nearby worktables. Afterwards, when reinstalled near assembler(s), it will upload its recipes to them.<br /><br />Blue cells are import range for the database.<br /><br />Uploaded recipes and bills will be lost if the database is moved or destroyed.<br /><br />I wonder what all these other buttons do...

### Assembler

|   | Size | Health | Power | Research Prerequisites | Resource Cost |
| - | ---- | ------ | ----- | ---------------------- | ------------- |
| <img src="https://github.com/zymex22/Project-RimFactory-Revived/blob/master/Textures/SAL3/smart_assembler.png?raw=true" width="96" height="96" /> | 3x3 | 250HP | 625W | Universal Autocrafting | 2x PRF Robotic Arm<br />1x PRF Machine Frame<br />120x Steel<br />10x Plasteel |

An automatic assembler controlled by a computer. Despite being called an assembler, it's also capable of simpler procedures such as cutting stone blocks, and refinery work.<br /><br />Downloads recipes from an adjacent recipe database.<br /><br />White cell is input range, Blue cell are db range, Yellow cell is output

### Adaptive Assembler

|   | Size | Health | Power | Research Prerequisites | Resource Cost |
| - | ---- | ------ | ----- | ---------------------- | ------------- |
| <img src="https://github.com/zymex22/Project-RimFactory-Revived/blob/master/Textures/SAL3/correcting_assembler.png?raw=true" width="96" height="96" /> | 3x3 | 350HP | 700W | Self Correcting Assemblers | 2x PRF Robotic Arm<br />1x PRF Weak AI Chip<br />1x PRF Machine Frame Large<br />10x Plasteel<br />150x Steel<br />2x Component Industrial |

An automatic assembler controlled by a primitive AI.<br /><br />The simple artificial neural network enables it to learn; to be more precise and efficient at individual recipes. Slowly overwrites currently unused recipe algorithms, as it has limited processing and memory capacity.<br /><br />Downloads recipes from an adjacent recipe database.<br /><br />White cell is input range, Blue cell are db range, Yellow cell is output

***

### Assembler / Recipe Database Usage
Once you have built, for example, a Machining Table; build or place a Recipe database adjacent to the table. Once built or placed, click on the Recipe database and observe the "Import recipe" action. Clicking that will open a contextual menu showing you the recipes available in the Machining Table. Clicking on any of those recipes will begin the importing process, that process will  take time.

Once you have imported one or more recipes into the Recipe database, you can place it adjacent to either an Assembler or Adaptive assembler. This, in turn, will allow the adjacent  assembler(s) to use the recipes from the Recipe database to setup bills as if it were the initial Machining table.