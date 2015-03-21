## Naming conflicts ##

If you encounter build errors while trying to compile **gpick**, chances are that your Lua library is named differently and **pkg-config** can't find correct ".pc" file. Makefile expects "lua5.1.pc" file, but in your case it can be called "lua.pc" or some other name.

Solutions:
  * You can use LUAPC variable to specify correct Lua name, so instead of usual "make" you can write "make LUAPC=lua". If you do not want to type this every time you compile **gpick**, you can set environment variable named LUAPC to correct name
  * You can create a symbolic link named "lua5.1.pc" pointing at your actual file