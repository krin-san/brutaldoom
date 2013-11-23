Brutal Doom
==========

Prepare to see the most disturbing, sadistic and morbid manifestation of violence that you ever seen in your life. This is the definitive gameplay enhancement mod for the GZDoom and Zandronum engines.

https://github.com/idk/brutaldoom

[linuxdistrocommunity][6]

Install:
--------
    $ wget https://raw.github.com/idk/brutaldoom/master/PKGBUILD -O /tmp/PKGBUILD && wget https://raw.github.com/idk/brutaldoom/master/brutaldoom.install -O /tmp/brutaldoom.install && cd /tmp && makepkg -sfi PKGBUILD && cd

Depends on: zandronum and doomseeker

    pacaur -S zandronum doomseeker

Setup:
------

Ensure all of your existing .wad files use lowercase only, no UpperCase allowed.

Copy your existing .wad files to ~/.zandronum/:
    
    cp *.wad ~/.zandronum/

Usage:
------

    zandronum &

Or for Multiplayer:
-------------------

    doomseeker &


Hashes:
-------

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

[6]: http://www.linuxdistrocommunity.com
[7]: https://github.com/idk/brutaldoom/issues