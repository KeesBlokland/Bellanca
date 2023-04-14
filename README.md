# Bellanca
These files are basically what Kai created, using the previous work from Albert. I just cleaned them up for my own use. (FreeCAD version 0.20.0 on Ubuntu-latest)

I imported the Step files, but for reasons unclear, there appear to be multiple copies of everything. So, just removed all the extra stuff, so that I have a normal working set. 

Since I rebuild my router (hardware is a StepFour) to get rid of all the windows stuff, and I would like to start using FreeCad in ernest, this project will do just fine to teach me ;-)

Source: https://github.com/Kailee71

Discusion here: https://www.rc-network.de/threads/fr%C3%A4sdaten-bellanca-super-decathlon.11947862/

From what I can see and deduct, this project has a very long history, sadly not everything is known to everybody. But one thing is sure, the amount of hours that went into this, is staggering! Something you don't appreciate until you do it yourself.

Thanks for all your hard work Kai and Albert!



I got my Stepfour Router many, many moons ago, but it used WindowsXP/XpertMill software, and dated hardware. Recently I upgraded all the hardware, things are now running on a RaspberryPi4 (cost me 75Euro's in the good days) with an SSD drive. The Controller board is from Planet-CNC, and the actual motordrivers are simple off the shelf stuff. (will look that up later). The first results are promissing, the router is at least twice as fast as before!

14 Apr 2023: Below is very much work in progress, I am updating as I work out the best method for getting from electrons to parts i can touch.

My present workflow from Drawings to Parts. 

I do a lot of work with Shapr3D for my 3D-Printing jobs, I am quite comfortable with it's use. However, my Ipad is struggling with the complete assembly. Therefore I decided to just use the subassemblies for now. 

- Loaded sub assemblies in FreeCAD, and removed any duplicates that could have been introduced by the conversion from Kai's Catia work to .stp files. 
- Saved that assembly as standard FreeCAD file with FCStd extension.
- In FreeCAD, take an assembly (f.i. Empenage) and select only the bits I need (3mm, 6mm, GRP, Jigs) and export to .step
- Import those .step files into Shapr3D, and play around. (modify, arrange flat, etc.)
- Shapr3D exports to .DXF for further processing. 

Next I need something in the middle that modifies my cutfiles to take care of the offset for the router bits. At present I am trying DeskProto. (But maybe this can be done in FreeCAD, I have not looked at that) I might simply try to use Shapr3D and enlarge all parts with 1/2 my milling bit.  
 
- Also need something to position all the parts. (Again, Shapr3D would be my prefered method)

- PlanetCNC drives my Router, it understands DXF, and could do the tabs as well. 


