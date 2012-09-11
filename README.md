pxd5_for_linux
==============

A library and editor for the Korg Pandora PX5D on Linux.

The Pandora PX5D is a portable multi-effect for guitar made by Korg. 
It is an amazing tool for guitar and bass players, has an audio USB interface to use it as a 
sound card which works out-of-the-box on Linux, and a USB-MIDI interface for which support has 
been added since Linux Kernel 3.0, allowing to use the Windows editor made by Korg via Wine and 
allowing to start implementing a native Linux editor.

This project aims to build a small library to be able to connect to the PX5D, edit and change presets.
First, mimicing the Windows editor from Korg will be the priority, then new features not preset
on the windows version could be implemented (relay standard midi program change, link MIDI controllers to
parameters, ...)

A QT GUI is also in progress.

The project relies on the following libraries:
- QT
- ALSA
- pthread

which should allow easy compilation for most distributions.

Current Status of the project:

* Library & GUI set up
* Pandora detection and connection working
* Getting current program number, name and enabled modules work.
* Changing programs work

Next on the TODO list:

* handle visualisation & edition of amp settings
* handle visualisation & edition of cabinet settings
* handle visualisation & edition of modulation settings
* handle visualisation & edition of delay settings
* handle visualisation & edition of reverb settings
* handle visualisation & edition of noise redution settings
* handle saving/loading all presets to disk
* handle the drum machine
