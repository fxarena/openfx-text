# openfx-text

Advanced internationalized cross-platform [OpenFX](http://openeffects.org/) text generator for Natron, Nuke, Resolve, Fusion and Vegas.

This project is a continuation of the Text node in Natron (from [openfx-arena](https://github.com/NatronGitHub/openfx-arena)), but with focus on cross-application support, better maintainability and more experimental features.

Currently under development, not end-user ready yet.

## Compatibility

* [Natron](https://natrongithub.github.io/) *2+*
* [The Foundry](https://www.foundry.com/) [Nuke](https://www.foundry.com/products/nuke) *7+*
* [Blackmagic Design](https://blackmagicdesign.com) [DaVinci Resolve](https://www.blackmagicdesign.com/products/davinciresolve) *15+*
  * Only works in the "Fusion" tab
* [Blackmagic Design](https://blackmagicdesign.com) [Fusion Studio](https://www.blackmagicdesign.com/no/products/fusion) *9+*
  * version 9 has issues with render scale
  * version 16 has issues with render scale, disable auto proxy
* [Sony](http://www.sonycreativesoftware.com)/[MAGIX](https://www.magix.com)‎ [Vegas Pro](https://www.vegascreativesoftware.com) *12+*

## Windows

TBA

## macOS

TBD

## Linux

### Requirements:

 * cmake and pkg-config
 * OpenGL development files and libraries
 * fontconfig development files and libraries
 * pangocairo development files and libraries

On Ubuntu install the following packages:

```
sudo apt install build-essential cmake pkg-config libfontconfig1-dev libcairo2-dev libpango1.0-dev libgl-dev
```

On RHEL/CentOS/Fedora install the following packages:

```
sudo yum install gcc-g++ cmake3 pkg-config fontconfig-devel cairo-devel pango-devel mesa-libGL-devel
```

### Build and install:

```
git clone https://github.com/rodlie/openfx-text
cd openfx-text
git submodule update -i
mkdir build && cd build
cmake -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX=/usr/OFX/Plugins ..
make && sudo make install
```

## License

```
Copyright (C) Ole-André Rodlie <ole.andre.rodlie@gmail.com>

This program is free software; you can redistribute it and/or
modify it under the terms of the GNU Lesser General Public
License as published by the Free Software Foundation; either
version 2.1 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
Lesser General Public License for more details.
```
