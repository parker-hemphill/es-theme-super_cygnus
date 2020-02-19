The original Cygnus theme is really nice but I wanted something that more closely resembled the colors of SNES.  Therefore I created a tweak with new color options I've dubbed **Super Cygnus**.
Besides the color changes the most noteable difference is a tweak of the layout of the marquee and coverart so it won't overlap with videos and has a more appealing (IMO) centered layout.

To install simply ssh into RetroPie and run the following commands:
```
mkdir -p ~/.emulationstation/themes
cd ~/.emulationstation/themes
git clone --depth=1 https://github.com/parker-hemphill/es-theme-super_cygnus.git super_cygnus
```

### Super Cygnus theme config file  
There are two files included below by the config.xml file, one is a colorset, the other is a template.
Simply run `nano ~/.emulationstation/themes/super_cygnus/config.xml` and adjust which files are loaded.

#### Colorsets
super_cygnus.xml       <--- This is the 'Super Nintendo' themed colorscheme. **Default**
cygnus.xml             <--- This is the default blue colorscheme. Same as original.
mono.xml               <--- This is a black and grey colorscheme. Same as original.
terminal.xml           <--- This is a green colorscheme. Same as original.

#### Templates  
cygnus.xml             <--- Slight changes to layout of marquee and coverart from original. 
noboxart.xml           <--- Same as cygnus.xml but without boxart **Default**
nometa.xml             <--- No metadata, all text except gamelist removed. Same as original.
simpleart.xml          <--- Large art, no overlayed boxart or marquee images. Same as original.
simpleart-nometa.xml   <--- Minimal theme with just a gamelist and large art. Same as original.

I've tried not to stray too far away from the original theme and have included the original readme.md along with the original authors information.
### Original readme.md below ###
![splash](https://choccyhobnob.com/dl/img/cygnus/splash.jpg)  
  
## EmulationStation Theme: Cygnus  
Cygnus is a clean theme that displays large preview images, videos, marquees,  all title-oriented metadata and some useful user-oriented metadata. Cygnus comes in three colour schemes, 'cygnus' 'mono' and 'terminal'.  
  
**NOTE: Cygnus uses cutting edge features. You will need the latest official emulaionstation for the video, marquee, and carousel features to work correctly. Update from the RetroPie setup menu, manage packages, core, emulationstation.**  
  
### Installing Cygnus  
  
ssh onto your RetroPie install and enter the following:  
  
`mkdir -p ~/.emulationstation/themes`  
`cd ~/.emulationstation/themes`  
`git clone --depth=1 https://github.com/ChoccyHobNob/es-theme-cygnus.git cygnus`  
  
It will now be choosable from the ui options menu in emulationstation  
  
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
![Cygnus](https://choccyhobnob.com/dl/img/cygnus/cygnus.jpg)  
![mono](https://choccyhobnob.com/dl/img/cygnus/mono.jpg)  
![terminal](https://choccyhobnob.com/dl/img/cygnus/terminal.jpg)  
  
![basic](https://choccyhobnob.com/dl/img/cygnus/basic.jpg)  
![detail](https://choccyhobnob.com/dl/img/cygnus/detail.jpg)  
![video](https://choccyhobnob.com/dl/img/cygnus/video.jpg)  
  
### Credits  
All xml, and some images created by Steve Boswell (ChoccyHobNob).  
  
Based on the "Eudora" theme by AmadhiX, which is in turn based on the "Carbon" theme by Eric Hettervik, which is in turn based on "Simple" by Nils Bonenberger.  Some system logos and line art images are borrowed from these themes.  
  
The following fonts are used under the licenses included with the font files:  
"Titillium Web", "Adobe Blank"  
