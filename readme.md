![splash](https://raw.githubusercontent.com/FollyMaddy/media/main/animated_gif/themes/cygnus-blue-flames.gif)

## EmulationStation Theme: Cygnus - Blue Flames
Cygnus is a clean theme that displays large preview images, videos, marquees,  all title-oriented metadata and some useful user-oriented metadata. Cygnus comes in three colour schemes, 'cygnus' 'mono' and 'terminal'.

**NOTE: Cygnus uses cutting edge features. You will need the latest official emulaionstation for the video, marquee, and carousel features to work correctly. Update from the RetroPie setup menu, manage packages, core, emulationstation.**

### Installing Cygnus

#### _UPDATE: Cygnus is now included in the theme installer in retropie-setup so that's probably the easiest way to install it!_

ssh onto your RetroPie install and enter the following:    

`mkdir -p ~/.emulationstation/themes`    
`cd ~/.emulationstation/themes`    
`git clone --depth=1 https://github.com/ChoccyHobNob/es-theme-cygnus.git cygnus`

It will now be choosable from the ui options menu in emulationstation

#### DTEAM-1 Update
Cygnus_- Blue flames is based on the work of "ChoccyHobNob". 
Changes:
- More systems for Lr-Mess / MAMEDEV and +.
- I changed a lot of images and logos. I have added systems images with controllers. Originally we didn't see the joysticks/gamepads. 
- Also, I changed the background to blue flames.
-  I slightly changed the position of the videos, marquees and the 3D box
-  New default theme for uncovered systems (theme.xml)

Note:-
- Don't use OMXplayer.
- changes was apply only where you can read "cygnus - blue flames" 
- To do list: Add "mascots" where you only have the system and the logo and modify some logos for unchanged systems


### Cygnus theme config file
There are two files included below by the config.xml file, one is a colorset, the other is a template.
Valid changes you can make here are as follows.

#### Colorsets
cygnus.xml             <--- This is the default blue colorscheme.  
mono.xml               <--- This is a black and grey colorscheme.  
terminal.xml           <--- This is a green colorscheme.  

#### Templates
cygnus.xml             <--- All bells & whistles. Lots of metadata, lots of art.  
nometa.xml             <--- No metadata, all text except gamelist removed.  
simpleart.xml          <--- Large art, no overlayed boxart or marquee images.  
simpleart-nometa.xml   <--- Minimal theme with just a gamelist and large art.  

### Platform Specific Themes
Cygnus comes with a large number of defined systems, more than even the default carbon theme. these will either be used when you install the emulator for a sytem and add some roms or you can choose them yourself for your existing systems.

This is useful if you want to override the display of systems to match your region and things like that. For example, by default Cygnus uses a picture of the USA SNES console and logo for the snes system; you can chage this behaviour by telling it to use either the 'sfc' theme or the 'snes-pal' theme to get the correct console and logo for you.

Create a file in `/opt/retropie/configs/all/platforms.cfg` if it doesn't already exist. Edit the file and add lines to it in the format \<system\>_theme="\<themename\>" so in our example above I could add

`snes_theme="sfc"`  
or    
`snes_theme="snes-pal"`    

other useful ones are:-

`megadrive_theme="genesis"`    
`pcengine_theme="tg16"`    
`nes_theme="famicom"`    

There are lots of these, look at the folder names for a list of all the available systems!


### Screenshots
![model3](https://user-images.githubusercontent.com/84874218/126497724-00423b78-09cb-4cdc-847e-3db45dace42f.jpg)
![Jakks](https://user-images.githubusercontent.com/84874218/126497819-ed85726e-3084-482b-8165-79e64e8101bb.jpg)
![ColecoVision](https://user-images.githubusercontent.com/84874218/126497858-967b1bfd-66e4-4f71-83db-b806f6237f5c.jpg)
![MegaDuck](https://user-images.githubusercontent.com/84874218/126497908-c0dd90c2-57f3-48ac-a359-0adf12b71b8f.jpg)
![Konamih](https://user-images.githubusercontent.com/84874218/126498015-321bd69c-edf9-4a10-961a-3e2f504ff086.jpg)
![Tigerh](https://user-images.githubusercontent.com/84874218/126498044-b8ad4a6c-5e8f-44d2-939c-26d41ff9fa22.jpg)

### Credits
All xml, and some images created by Steve Boswell (ChoccyHobNob).

Based on the "Eudora" theme by AmadhiX, which is in turn based on the "Carbon" theme by Eric Hettervik, which is in turn based on "Simple" by Nils Bonenberger.  Some system logos and line art images are borrowed from these themes.

The following fonts are used under the licenses included with the font files:
"Titillium Web", "Adobe Blank"
