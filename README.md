# PocketDock
The Pocket Dock modular synthesizer system and associated modules

Licensed under CERN-OHL-P-2.0

The base Pocket Dock is designed to take the +/-12v audio and control voltage of a Eurorack or Pocket Rack synthesizer system and safely shift them down to interface with a Pocket Operator, while giving it a nice little cradle to sit in a modular system. I've also made other modules to fit the Pocket Rack standard. These are all still very much in progress. The Dock is based on interfacing with the Pocket Operator via pogo pins, but that has not proved to be reliable in testing; I'm looking for better solutions.

Here's a rundown of the modules.
## Power Distro
#### Not tested
Provide Molex connectors to split power to other Pocket Rack modules, with reverse polarity protection.
## Buffered Mult
#### Tested: works great
two 1-to-3 buffered multipliers in one module. The second input is normaled to the first, so when nothing is connected to Input 2, it acts as a 1-to-6 mult. This module also doubles as an unbuffered passive mult by not populating any components besides the jacks and closing all the solder jumpers.
## Clock Skipper
#### Tested: works on a breadboard, current PCB version has no audio output
A simple version of a gate sequencer that uses an incoming clock signal, and mutes or unmutes the signal based on a small bank of DIP switches.
##Noise Hits
#### Not tested
White, pink, and blue noise generator with a simple transistor VCA on each channel to act as a simple drum machine.
## Nyblcore and Pikocore
#### My PCBs are untested
A version of Infinite Digit's [Nyblcore](https://github.com/schollz/nyblcore) and [Pikocore](https://infinitedigits.co/docs/products/pikocore/) refactored into the Pocket Rack size.
## Pocket Socket
#### Not tested
A base for prototyping new modules. All the jacks and power circuitry are on the main module, and the actual audio passes onto a daughterboard with pin headers.
## Quant
#### Not tested
a Seeed Studio Xiao-based quantizer. I haven't started the firmware on this yet.
