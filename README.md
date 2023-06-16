#TouchOSC Performer for Bitwig (aka TOP)
A TouchOSC performer providing mixing, channel strip & clip launching functionality.  Designed & tested with Bitwig, probably works with Reaper.

##Background
This is a personal project that I’m making available to Bitwig & TouchOSC communities. It started when I was thinking about having a DAW-connected hardware mixer with motorised faders so that what I saw was what I got, but was put off by the size and cost.

It’s been designed / grown around principles of minimalism & simplicity: How few controls do I require to meet **my** needs, and what is the simplest or easiest way of achieving that? The config / code gets refactored as I find more elegant ways of doing this. Thanks to Hexlar for helping me find better ways!

It’s for use on tablets or other compatible touch screen devices with a similar, or larger, screen size.  I’ve tried to make all interactive design elements easy enough to hit with a finger tip, my reference device for this is my 10.4” 1800x1000 pixel Samsung S6 Lite. 

##Setup
**TOP for BW4** is for use with Bitwig v4.4.x – a version for Bitwig 5 will follow shortly

You will need to have:
-	Bitwig with an appropriate version of the [DrivenByMoss extension](https://www.mossgrabers.de/Software/Bitwig/Bitwig.html) installed and setup to talk with TouchOSC
-	
-	TouchOSC setup to talk to your PC and / or tablet or device
-	*Follow the respective manufacturer's instructions for these products*

DrivenByMoss OSC Config in Bitwig needs the following:
-	Value resolution = Low (128)
-	Bank Page Size = 8
-	Behaviour on Stop = Return to Zero
-	VU Meters = On
-	*All other setting as per your own needs*

##Features & Basic Use
-	Tracks & Clips follow your colour choices from Bitwig in all views

###Transport Bar (always visible)
-	Select from your projects already loaded in Bitwig 
-	Record (on armed tracks / clips)
-	Stop (returns to position zero)
-	Play (plays from last paused position, press again to *pause* at current position)
-	Position & Time counter displays
-	Current project’s Audio Engine activation status and toggle
-	Save the current project
-	Undo change
-	Redo change
-	Bitwig->TOP state synchronisation

###Navigator (always visible)
-	Enter / Exit a Group track (If the currently selected track is a group, currently only first level group works)
-	FX / Tracks toggle (switches between standard tracks and FX tracks)
-	Last / Next bank of 8 tracks (selects a bank of tracks)
-	Last / Next track (scroll the visible tracks backwards / forwards by one track)
-	Last / Next bank of 8 scenes (selects a bank of scenes)
-	Last / Next scene (scroll the visible scenes backwards / forwards by one scene)
-	Create a new scene from the currently playing clips

###Mixer
-	Master (always visible) and up to 8 additional visible tracks, each with; name, type, pan, volume, basic vu / activity meter, mute, solo, record arm
-	Track select by clicking on it’s name (selected track will flash briefly and then have corner outlines)

###Channel
For the selected track
-	Mixer (elements as above)
-	FX Send levels (for first 8 effect tracks)
-	Remotes for each of the track’s devices, each with; value dial, value display, name of remote
-	Quick navigation to select other tracks in the current bank whilst in this view
-	Navigation for devices and their remote pages

###Launcher
-	Layout is per Bitwig’s *Arrange* view, with Scenes in columns and Tracks in rows.
-	Playing clips are highlighted, queuing clips are shown with a border
-	Scene play (clicking on a scene’s name with play / queue all the clips in that scene)
-	Track stop (clicking on a track’s name will queue a stop for that track’s playing clip)
-	Clip play (clicking on a clip will play / queue that clip)

##License
This project is licensed under the MIT license



