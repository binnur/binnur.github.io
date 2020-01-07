# Project: Entry to 3D Printing with AdaFruit Gizmo Ornaments

I am a [FIRST Robotics Competition](https://www.firstinspires.org/robotics/frc) mentor. This year one of our students is interested in bling, so I saw an opportunity to step into the world of LEDs and blinking lights. Right prior to the Holiday Season, I decided to checkout [MicroPython](https://micropython.org) and did a quick setup for [CircuitPython](https://circuitpython.org) as it is an open source derivetive targeted towards students developed by [Adafruit](https://www.adafruit.com). It is definitely a fun development platform, and it got my creative juices flowing! 
  
During the Holiday Season, [Tarkan](https://www.linkedin.com/in/tarkan-al-kazily/) (our son) initiated me to 3D printing.  As part of the initiation he introduced me to the world of [Thingiverse](https://www.thingiverse.com) and I found [Adafruit’s Gizmo Ornaments](https://www.thingiverse.com/thing:4019946). What can be better than a blinking holiday ornament?! The first part of the article will cover my notes about 3D printing process, and later (when my electornics arrive) I will update the article with blinking lights.

## Our 3D Printing Setup
We have a [Monoprice MP Mini Delta 3D Printer](https://www.monoprice.com/product?p_id=21666) which Tarkan diligently maintains during his visits. Rest of the document I will abbreviate it  to MPMD.

3D printing is a process of making physical objects from a three-dimensional digital model, i.e. object’s CAD representation. The 3D printing process, also known as additive manufacturing, creates three dimensional objects by extruding materials, known as filament, layer by layer as specified by its model. 

Similar to PDF for document printers, 3D printers also require a digital document format for processing these 3D design files. MPMD supports STL format, which is also common among other 3D printers, for digital designs. As the 3D printing process is additive and layered, the file needs to be preprocessed by a slicing software which divides the 3D model into corresponding horizontal layers and saves as gcode for printer-ready. Gcode programming language is used by 3D printers that contains commands for controlling each action that 3D printer performs.

Given this, my setup required:
1. Selecting a CAD package for creating 3D model and exporting corresponding STL file. I installed [Autodesk Fusion 360](https://www.autodesk.com/campaigns/fusion-360-for-hobbyists) for hobbyists.
2. Installing [Ultimaker Cura](https://ultimaker.com/software/ultimaker-cura) for slicing the STL files and getting them ready to be printed by our 3D printer.
3. Cura does not support MPMD out of the box, so printer profile needs to be installed to ensure proper slicing of the 3D model/STL file to code that our printer understands. See [here](https://docs.google.com/document/d/1LHomAxmgSWEggiCM1p6B0vZCIcJPIFTe0OqnozhtZxc/edit) for detailed instructions. 
4. The printer profile can be further customized by providing a printer specific start and end gcode. Did I mention Tarkan was diligent at getting our printer to top shape? He also provided start.gcode to ensure a successful print, including needed calibration information.

### Tips/Techniques to Watch for
Internet is full of 3D files for printing. These can be opened in Cura and processed with slicer for 3D printing. Prior to printing, it is advised to slice and preview the model to ensure proper print. Specifically check for: 
* Quality of adhesion to the bed — *raft* setting will lay down a few base layers before printing the model to help it stick to the bed.
* Verify no overhangs, sharp angles, or free floating sections — *support* setting will provide props to support the proper printing of the model.

I also recommend good SD card organization and clear file names for the digital files as you’ll likely reprint these parts at a later time.  

## Review of the 3D Prints



## Next Steps
* I like to get comfortable enough with Fusion 360 for modifying existing designs and making my own. Other than spending time in the application, I plan to checkout the coursera class...