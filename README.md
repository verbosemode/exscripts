#exscripts

This repository contains some of the scripts I've written for [Exscript][].

!WARNING! I don't take any responsibility if those scripts screw up your network or fry your favorite pet by accident.

I encourage you to run those scripts first in your testlab or on one or two hosts. Automation is great for saving time but I can also mess up your whole network within seconds!


##Scripts

###update-ios.exscript

* Copies an IOS image from a HTTP server to an IOS device if there is enough space on the flash
* Sets the boot image to the uploaded image if the md5 checksum matches
* You might need to replace the URL in the script
* It doesn't initiate a reload (yet)

Right now it only contains 5 different Catalyst images as an example. Adding new IOS images  is a bit messy. Just send me a patch if you figure out how this script can be simplified. At the moment the exscript code is generated from anther Python script. Maybe I'm also going to rewrite it completely in Python.

###reload-ios.exscript

* Reloads the device if a specific image is in the flash file system
* Will add more options in the future to decide when to reload a device

[Exscript]: https://github.com/knipknap/exscript "Exscript"




