# Introduction #

This file is a self-extracting archive and will prompt for the target folder on execution.

# Details #

It has the following bug fixes:
- when using absolute time in capture file the ‘,’ would not be inserted, result is that the first 2 columns become 1
- corrected trouble code reading routine for MY99/00 ECUs
- fixed startup thread activity after ecuQuery/ecuFlash tools

It has the following additional features:
- raw ROM format check for ecuFlash tools
- manifold relative pressure (corrected), this item will overcome the 1.27b (18.42PSI) limit of the traditional Manifold Relative Pressure parameter.
- redesigned com port frame
- ecuQuery functionality to read RAM memory between 2 supplied addresses
- ecu definitions for MY06 models
- support for OpenPort 1.2 hardware