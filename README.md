Brutal Doom
===========

[Brutal Doom][8]

Prepare to see the most disturbing, sadistic and morbid manifestation of violence that you ever seen in your life. This is the definitive gameplay enhancement mod for the GZDoom and Zandronum engines.

![Brutal Doom](https://raw.github.com/idk/brutaldoom/master/cover.jpg)
https://www.youtube.com/watch?v=nzsG2sLc7dk&t=1m31s

Includes:
---------

[Version 19][9]

[Doom Metal Soundtrack Mod Volume 4][10]

Depends:
--------

    pacaur -S zandronum doomseeker

Install:
--------

	mkdir -p ~/abs/brutal19
	cd ~/abs/brutal19
    wget https://raw.github.com/idk/brutaldoom/master/PKGBUILD && wget https://raw.github.com/idk/brutaldoom/master/brutaldoom.install  && makepkg -sfi PKGBUILD

Setup:
------

Run 'zandronum' to initialize: (Click cancel after it fails to open if required)

    zandronum

Ensure all of your existing .wad files use lowercase only, no UpperCase allowed.
Now copy your existing .wad files to ~/.zandronum/:
    
    cp *.wad ~/.zandronum/

Now copy zandronum.ini to ~/.zandronum/:

    cp /usr/share/games/brutaldoom/zandronum.ini ~/.zandronum/zandronum.ini

Usage:
------

    zandronum &

Or for Multiplayer:
-------------------

    doomseeker &

Hashes:
-------

	brutal19.zip 5b87f3a849fc61561fc971c24c1cc2840fc42e063ef2a946cfd11dc77a3d0cbd310750836f2b1b8be86e1c3211a1b426447ef2917caef3adc8cbef50f6f321b2

	DoomMetalVol4.zip b1180910025e8b8f065c56518fb1556678ef5c6062dc527e1f3e54dfa039e82f8e49bb1997ccf06a07e451576fbe35c321773eb7dbb7f62b1654b59cb9e07f32

    brutalv018a.zip fc0d6f2a63aeb3f9028221bd9ab77ec5
    
    doommetalvol4.wad 67975e13059aceb7fa5d93d3d91de99b

Contributing:
-------------

1. Fork it.
2. Create a branch (`git checkout -b my_brutaldoom`)
3. Commit your changes (`git commit -am "Added foo and bar"`)
4. Push to the branch (`git push origin my_brutaldoom`)
5. Create an [Issue][7] with a link to your branch
6. Join the Linux Distro Community IRC or Mumble! :D

SHARE AND ENJOY!
----------------

I have nothing to do with making this mod I only make package for my Arch Linux. :)
 Is version 18a cause I cannot get 19 to work, some error about something or other. :P

[linuxdistrocommunity][6]


[6]: http://www.linuxdistrocommunity.com
[7]: https://github.com/idk/brutaldoom/issues
[8]: http://www.moddb.com/mods/brutal-doom
[9]: http://www.moddb.com/downloads/brutal-doom-version-181
[10]: http://www.moddb.com/mods/brutal-doom/downloads/doom-metal-soundtrack-mod-volume-4