# Standard Arduino libraries for Ctags

This repository contains a copy of the standard Arduino libraries. This is useful
for creating Ctag-files because you normally cannot access the built-in libraries
like Wire.h for that matter.

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

## Licence note

These libraries are licenced under the GNU LGPL Version 2. A copy of that can be
found in the LICENSE file.