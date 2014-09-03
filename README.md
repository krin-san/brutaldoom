Brutal Doom
===========

[Brutal Doom][8]

Prepare to see the most disturbing, sadistic and morbid manifestation of violence that you ever seen in your life. This is the definitive gameplay enhancement mod for the GZDoom and Zandronum engines.

![Brutal Doom](https://raw.github.com/idk/brutaldoom/master/cover.jpg)
https://www.youtube.com/watch?v=nzsG2sLc7dk&t=1m31s

Includes:
---------

[Version 18a][9]

[Doom Metal Soundtrack Mod Volume 4][10]

Depends:
--------

    pacaur -S zandronum doomseeker

Install:
--------

	mkdir -p ~/abs/brutal18a
	cd ~/abs/brutal18a
    wget https://raw.github.com/idk/brutaldoom/master/PKGBUILD && wget https://raw.github.com/idk/brutaldoom/master/brutaldoom.install && makepkg -sfi

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

    brutalv018a.zip c940afc94317937b9b91da071440053d426b82a43d9f756aa2b3c899d7e966da06cc2d4226258f5b074ea2da780043a5cecfa2e0ba9e21d4c0aee14d282e8d60
    
    DoomMetalVol4.zip b1180910025e8b8f065c56518fb1556678ef5c6062dc527e1f3e54dfa039e82f8e49bb1997ccf06a07e451576fbe35c321773eb7dbb7f62b1654b59cb9e07f32

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