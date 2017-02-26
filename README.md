# Standard Arduino libraries for Ctags

This repository contains a copy of the standard Arduino libraries. This is useful
for creating Ctag-files because you normally cannot access some of these built-in 
libraries like Wire.h.

**Important:** Do not use these Libraries for your Arduino sketches, as they
might be outdated or even incompatible with current versions of the Arduino
compiler.

## Generating a tagfile

To generate the tagfile, open a terminal in the libraries folder of this
repository and run 

`arduino-ctags -R .`

## Extending your tagfile

If you want to create tags for additional libraries, just copy them into the 
`libraries` folder of this repository before execution of the `arduino-ctags`
command. Then they will be included automatically.

## Note on the WiFi library

Due to the big size and contents of the WiFi library, it removed from the
repository. This helps to keep file size reasonable. If you want to use WiFi 
capabilites, move the `WiFi` folder from your Arduino projects folder to 
`libraries`

## Licence note

These libraries are licensed under the GNU LGPL Version 2. A copy of that can be
found in the LICENSE file.