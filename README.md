# openfx-text

Advanced internationalized [OpenFX](http://openeffects.org/) text generator for [Natron](https://natrongithub.github.io/), [The Foundry](https://www.foundry.com/) [Nuke](https://www.foundry.com/products/nuke), [Blackmagic Design](https://blackmagicdesign.com) [DaVinci Resolve](https://www.blackmagicdesign.com/products/davinciresolve) / [Fusion Studio](https://www.blackmagicdesign.com/no/products/fusion).

This project is a continuation of the Text node in Natron (from [openfx-arena](https://github.com/NatronGitHub/openfx-arena)), but written from scratch with focus on cross-application support and more experimental features.

Currently under development, not end-user ready yet.

## Windows

TBD

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

### Build and install:

```
git clone https://github.com/fxarena/openfx-text
cd openfx-text
git submodule update -i
mkdir build && cd build
cmake -DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX=/usr/OFX/Plugins ..
make && sudo make install
```

## License

```
Copyright (C) 2019, 2020 Ole-André Rodlie <ole.andre.rodlie@gmail.com>

This program is free software; you can redistribute it and/or
modify it under the terms of the GNU Lesser General Public
License as published by the Free Software Foundation; either
version 2.1 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
Lesser General Public License for more details.
```