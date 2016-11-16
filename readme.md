# Striation
A Theme for EmulationStation and RetroPie


About
-----

Based on the wonderful and versatile Eudora theme by AmadhiX, Striation has four goals in mind:

- Overall larger text for living room scale, widescreen displays
- A simple and clean design with larger boxart and maximized metadata
- As small a file size as I can manage (currently just over 4mb)
- A unique design for each system/platform (more below)

The name Striation comes from the patterns seen in nature from fault movement, but really it's just a cool word for stripes. My high concept for the theme is two-fold. As you scroll through the main menu of Emulation Station the logos displayed for each system resemble those found on the original hardware box. 

Selecting a system is then like opening that box with a background of stripey colors weighted to resemble the hardware and a logo to match. In many cases this means that the main menu logo and the system logo are different. I've found it enlightening and challenging to create many of these rarely seen variations but mostly I think it looks fantastic. If this is bothersome to you it's very easy to customize the images so jump down to the CUSTOMIZATION section below.

Now in Two *Exciting* Varieties!
------
Early on I had someone comment that they'd like to see the user metadata incorporated for 'times played', 'last played' and 'rating'. Thanks to that request there are 2 varieties of Striation, one with and one without the user metadata. Take your pick!

[Striation **Without** User Metadata](https://github.com/ShawnS52/es-theme-striation) on Github ([zip version on Dropbox](https://goo.gl/LTawWo))


[Striation **With** User Metadata](https://github.com/ShawnS52/es-theme-striation-usermeta) on Github ([zip version on Dropbox](https://goo.gl/rIaLq0))


Preview
------
For more [view my album on Imgur](http://imgur.com/a/50PsR) or check it out in action on [YouTube](https://www.youtube.com/watch?v=isNlcEnvw1k).


![Image](http://i.imgur.com/7X6GVer.jpg)
*Main Menu View*

![Image](http://i.imgur.com/7mfsKP7.jpg)
*Super Nintendo WITH UserMeta (Landscape Layout)*


![Image](http://i.imgur.com/2UIXWxB.jpg)
*Super Nintendo WITHOUT UserMeta (Landscape Layout)*


![Image](http://i.imgur.com/vuRfh1H.jpg)
*Sega Genesis WITH UserMeta*

![Image](http://i.imgur.com/AauV605.jpg)
*Sega Genesis WITHOUT UserMeta*

![Image](http://i.imgur.com/U5AkbQJ.jpg)
*Simple Layout used in both versions of Striation*


Layouts
------
Like Eudora, I've done my best to match theme layouts with each system to maximize the boxart images. There are 3 types in the NO Usermeta version and they're also easy to customize depending on your region or needs. There's **Portrait**, **Landscape** and **Landscape-SquareBox**. 

The SquareBox version is great for platforms that had uniformly square boxes and gives the metadata some extra room to breathe. Unfortunately, most platforms require the Landscape layout since the boxes varied wildly between regions. If you're on a 4:3 display you'll also probably want to use the Landscape layout, things get pretty cramped otherwise.

Like Eudora, the rating, last played timestamp, and play count have been omitted from the base theme. I've had requests to enable them. We'll see how that goes, maybe in an additional release.

**NOTE:** *For the UserMeta version of the theme there is no wider Landscape layout. To accommodate the user metadata and the game details I squeezed the boxart down to the "Squarebox" size.* It limits the size of the boxart which was one of my original goals but it's a decent balance between screen space for all the details.


What's Included
------

Here's the breakdown of what's covered based on the [supported systems](https://github.com/retropie/retropie-setup/wiki/Supported-Systems) on the RetroPie Wiki:

**Fully Themed:**
- 3do
- Amiga
- Amstrad CPC
- Apple II
- Atari 2600
- Atari 5200 and 8 bit series
- Atari 7800
- Atari Jaguar
- Atari Lynx
- Atari PC (ST/STE/TT/Falcon)
- Colecovision
- Commodore 64
- Daphne
- Dragon 32
- Dreamcast
- Famicom Disk System
- FinalBurn Alpha
- GameCube
- Game & Watch
- Game Gear
- Game Boy
- Game Boy Color
- Game Boy Advance
- Genesis
- Intellivision
- KODI
- Macintosh
- MAME (lr-mame, mame, mame4all, advancemame)
- Master System
- Mega Drive
- MSX
- Nintendo 64
- Nintendo DS
- Nintendo Entertainment System
- Neo Geo
- Neo Geo Pocket
- Neo Geo Pocket Color
- Odyssey2
- PC
- PORTS
- PlayStation 1
- PlayStation 2
- PlayStation Portable
- RETROPIE (settings menu)
- Saturn
- Sega 32X
- Sega CD
- Sega SG-1000
- Super Nintendo Entertainment System
- TurboGrafx-16
- Vectrex
- Virtual Boy
- Wii
- WonderSwan
- WonderSwan Color
- ZX Spectrum

**Partially Themed** (pre-existing logos included, generic background):

- CoCo
- ScummVM
- Steam (added by special request)
- Super Mario War
- Wine (added by special request)
- Zmachine

**Not Themed**(I hope to release European, Japanese and "Old PC" updates someday):

- Adventure Game Studio
- Nintendo (Famicom, Super Famicom)
- Oric (Oric-1, Oric Atmos, Stratos/IQ164, and Oric Telestrat)
- PC Engine
- ResidualVM
- SAM Coupé
- Sega (Mega CD, Super 32X)
- TI-99/4A
- TRS-80
- Videopac


Preview Image Size
------

Again, like Eudora: you may wish to set your scraper to pull larger image files.  If you are using sselph's scraper, you can use the -max_width parameter to do this, matching the width of each system's layout.

Rough maximum sizes are as follows for each layout template:
- Portrait:	400x600px
- Landscape: 600x400px
- Landscape-SquareBox: 600x600px


Customization
------

Say you only have Super Famicom games in your ROM folder or you've separated the Japanese Sega Mega-CD from its American cousin, the Sega CD. This will rule out the extreme variations in boxart so you can switch the layout of each system if you'd like. Just head into each system's folder located in:

	"themes/striation/SYSTEM_NAME/theme.xml"

and change the following line as desired:

	<include>./../common/templates/portrait.xml</include>

change it to **portrait**, **landscape** or **landscape-squarebox**


If my alternate logos bug you just change the filename in the same .xml file from "logoconsole.svg" to "logo.svg". This will match the logo on the main menu:

	<view name="basic, detailed">

	<!-- System Specific Images -->

		<image name="logo">

			<path>./logoconsole.svg</path>


Credits
------

"Striation" is created by ShawnS. You can find me:

- on the [RetroPie forums](https://retropie.org.uk/forum/user/shawns)
- on the [RetroPie reddit](https://www.reddit.com/user/ShawnS52)
- on my own little slice of the Internet at [GameLuv.com](http://gameluv.com)

Based on the "Eudora" theme by AmadhiX which is in turn based on the "Carbon" theme by Eric Hettervik, based on "Simple" by Nils Bonenberger.  Many system logos are inherited from these themes but have been altered or replaced with custom variations.

The following fonts are used under the licenses included with the font files:

"Open Sans" (Bold, Regular and Semibold) by Google.

"Adobe Blank" maintained by Dr. Ken Lunde.


Changelog
---------

2016-11-16

v1.0 Initial version

