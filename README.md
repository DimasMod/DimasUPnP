# ~~WaifUPnP~~ Dima's UPnP
This is a fork of WaifUPNP, made to change the build system, set up GitHub packages and rebrand (because of professionalism).
Why? [A networking library](https://github.com/DimasMod/JRakNet) used by the Java version of Dima's Mod kernel has a dependency of WaifUPnP, 
and the original project has the following problems:
- It uses the "ant" build system
- It doesn't have a maven repository
- It has a questionable name

What this fork does to address these issues?
The following:
- Changes the build system to use Gradle
- Renames the project
- Adds a GitHub workflow to build maven packages pushed to the GitHub maven repository
It also does these little tweaks:
- Fixes two typos: `_extermely_` -> `_extremely_` (credits to this [PR](https://github.com/adolfintel/WaifUPnP/pull/18)) and `an UPnP` -> `a UPnP`
- implements custom app names (credits to this [PR](https://github.com/adolfintel/WaifUPnP/pull/22))

## Original README.md

UPnP Port Forwarding for Java couldn't be any easier!

WaifUPnP is an _extremely_ lightweight Java library that allows you to:

- open/close TCP/UDP ports
- check if there's a UPnP router available
- check if a port is already mapped

using literally 1 line of code, as it should be! 

It's as easy as:

```java
UPnP.openTCP(<port number here>);
```

Usage Examples are included.

## Usage

To compile, import the project in Netbeans.
Alternatively, download the binaries from http://fdossena.com/?p=waifupnp/index.frag

Once you have the .jar files:

- Import `WaifUPnP.jar` into your application
- Optionally, import `WaifUPnP-javadoc.jar` if you need JavaDoc
- `WaifUPnP-sources.jar` contains the source code and should not be imported into your project

## Compatibility

Java 6 and newer

## Limitations

WaifUPnP is a very basic implementation of UPnP, that only scans for the default gateway, and can only open/close ports.

While this is enough for most people, if you need a full implementation of UPnP, you should take a look at [Cling](http://4thline.org/projects/cling/)

## License
Copyright (C) 2015-2018 Federico Dossena

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Lesser General Public License as published by
the Free Software Foundation, either version 2.1 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU Lesser General Public License
along with this program.  If not, see <https://www.gnu.org/licenses/lgpl>.
