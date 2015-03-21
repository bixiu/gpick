gpick uses SCons build system, so first of all you need SCons installed (http://www.scons.org)

Check that you have all required [dependencies](BuildingDependencies.md)

Typing `scons` should successfully compile all source files and create executable file in _build/source_ directory

You can actually run gpick without installing it, just type _./build/source/gpick_ (Linux) or _build/source/gpick.exe_ (Windows)

Installation is operating system dependent:
  * Windows
    1. typing `scons nsis` will write gpick version information into NSIS script
    1. now you can compile NSIS script file _installer/script.nsi_
    1. use generated installer file to install gpick
  * Linux
    1. typing `scons install` will install gpick into default installation directory _/usr/local_ (most probably root access will be required). If you want to install into different directory, you can do it in two ways:
      1. type `scons install DESTDIR=/mydir` where `/mydir` is your directory
      1. create a _user-config.py_ file in project directory and write the following into it: `DESTDIR="/mydir"` where `/mydir` is your directory. Now typing `scons install` will install gpick into your directory
    1. you will have to type `update-menus` to add gpick entry to your menu