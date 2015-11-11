# RetroPie-Silent
Basic configurations to silence all system outputs for RetroPie 3.0

Please execute the following command line to silence various outputs:
```
$ sudo ./retropie_silent.sh
```

## System Outputs
This will turn off the following outputs

### Raspian
* Boot logo
* Kernel messages
* Voltage warnings
* Temperature warnings
* Rainbow splashscreen
* Terminal blinking cursor

### X11
* Cursor

### Libretro
* OSD (On Screen Display)

### RetroPie
* Splash screen (disables service)

### EmulationStation
* Loading messages

## Additional Options
This will also set the following options
* Turn off boot delay
* Force sound over HDMI
* Disables exit from EmulationStation

## Additional Files
This repository also contains several diffs in case you want to recompile this packages.

### SysVinit
These diffs removes any broadcast warnings from the `shutdown` command.
Never apply these diffs to any multi-user system or some people will punch you in the face!
* `shutdown.c.diff`
* `initreq.h.diff`

### EmulationStation
* `Renderer_init_sdlgl.cpp.diff` Disables the cursor earlier to prevent flicker
* `Window.cpp.diff` - Removes the splash screen from EmulationStation (which normally can't be disabled by design [1])

----
[1] https://github.com/Aloshi/EmulationStation/issues/203
