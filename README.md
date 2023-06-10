# ludwig

complete and visually pleasing moss osc template.

You _need_ :
- a recent bitwig and latest drivenbymoss extensions
- a valid touchosc setup (fairly well explained on youtube)

## major changes

### `0.1a` : first public release

ditto

### `0.2` : implement better looking fader

- version code in xml now (new in touchosc desktop version)
- GUI fader pots (thanks to RahulDJ on "TouchOSC templates makers" facebook community
- general fader "block" rework
- better color logic (unified across the whole project)
- fix some font render issues (related to touchosc font engines)
- address new clip launcher behavior (bitwig5)
- Colors on user mapping to better differentiate them with bw gui

## features

- Reliably working touchosc environment, featuring most mixing oriented features.
- vu-meters with clip display
- complete metadatas (metric, names, color)
- watch modulated controls in real time where it matters
- check your markers at a glance
- devices control across pages
- complete send matrices (even across layers)
- full clip view
- fast (really)
- eye-candy

## setup

Install drivenbymoss extension. Set IP addresses.

- Resolution **must** be set at 1024 (medium)
- Bank **must** be set to 8 (this is the default)
- other stuffs can be set to your taste

## mixer

You should not be too lost here :)

- 🔴 : arm track
- 🎧 : solo/cue
- ❌ : mute track
- 📢 : monitor track
- 🟩 : automonitor

You can select a track by tapping its name (top, corner edges show currently
selected track).

You can scroll across pages in the mixer using the red arrows 
in the bottom right (⚠️: this changes current track selection)

### send panel

Tap and hold "send" rectangle button (at the right side of the fader), in order to
display the send faders of a track.

Be careful not to be "holding" the fader when releasing the send button.

### groups

You can "dig" a group by tapping "group" under the pan knob.

If you're already inside a group, you can get back to its parent using the 
"rewind" (⏪) at the left of the 1st track title

## device

Control the currently selected device.

### icons (top left)

- 🟠 : bypass
- 📌 : pin the device
- ➕ : maximize device
- 🎮 : display the "8-knob" section
- 🔲 : display the popup window (3rd parties, eq, grid, ...)

Your too many pages can be browsed on the upper right

The other effects on the same "track" are on the bottom

You can also access neighboring track and layers from the vertical
menu on the right

Access the layers' mixer with the 🟥button at the very bottom.

The layer mixer will pop from the left. It behaves like the main
mixer (refer to this section)

### clips

Tap a clip to play it

Tap an empty clip or the stop button at the bottom to stop.

Red arrows scroll 8 scenes, orange arrows scroll 1 scene at a time.

### mappings

cues are the timeline marks you're adding on your timeline, displayed in chronological
order. (use the red arrow to page across those if you have that many)

mapping the tiny orange hand on the Bitwig' window's bottom right, just a bunch of 
custom fader for you. they still display their names and modulation status.

## misc

The right side of the screen has some global widgets (top to bottom)

- the green bar at the top is the master vu.
- 🟢: forces an update, bitwig will send its entire osc state, use this in case of crash
- purple square : current tempo
- blue square : current beat
- yellow square : current time (minutes/seconds)
- green square : **PLAY**
- red square : **REC**
- blue square : loop
- Red arrows : scroll the mixer and clips (8 tracks at a time)
- orange square : master mute

## non features

(stuffs this project is not about)

- live loop recording
- features outside of current bitwig' OSC API
- anything bloaty (if it's not easily implemented path/messaging, it doesn't belong here)
- the longer goal is a performance tool, this means : 
  - no tiny screen support
  - no legacy support (touchosc is very fast and reliable on many stuff though)
  - no "discoverability"

- Feel free to open issues.
- Feel free to fork the project 
- (but don't submit PR until I can figure some way to version the template as an XML file, tosc is to painful)

## todo

implements features around the AltMode (new in bw5) for many controls.

  
