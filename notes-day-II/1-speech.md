Worms-style terrain with jaws.js - Ippa
=======================================

*Chingu* - Ruby game engine
*UnitJS* - Clientside web framework
*Jaws.js* - JS 2D game framework

2D Canvas, Open source, no deps, about 50kB

### Why 2D Canvas
- usually accelerated through 3D-hardware
- many browsers support
- based on game states (public methods: setup/update/draw)
- adding assets

Worms-style terrain it's an image
you can paint your level and the worm will interact with the level...

### Basics
We need to get ability to get each pixel on the screen to do the collisions
every pixels is represent by 4 int R/G/B/Alpha

PLAY: http://jawsjs.com/ongamestart

### Step 1 - one pixel on the bottom of square for collision detection

### Step 2 - all pixels around bounding box for collision detection

### Final - destructive terrain

- no soft brushes
- lossless format for colors


Homepage: http://ippa.se/
