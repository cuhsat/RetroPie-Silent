# RetroPie Silent
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

### Libretro
* OSD (On Screen Display)

### X11
* Cursor

### EmulationStation
* Loading messages

### RetroPie
* Splash screen (disables service)

## Additional Options
This will also set the following options
* Force sound over HDMI
* Turn off boot delay

## Additional Files
### SysVinit
This repository also contains the files `shutdown.c.diff` and `initreq.h.diff` to remove any broadcast warnings from the `shutdown` command. *NEVER* apply these diffs to any multi-user system!

### EmulationStation
This repository also contains the file `Window.cpp.diff` to remove the splash screen from EmulationStation (which normally can not be disabled by design [1]).

----
[1] https://github.com/Aloshi/EmulationStation/issues/203
