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

### X11
* Cursor

### Libretro
* OSD (On Screen Display)

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
This repository also contains the files `shutdown.c.diff` and `initreq.h.diff` to remove any broadcast warnings from the `shutdown` command. **Never** apply these diffs to any multi-user system or some people will punch you in the face!

### EmulationStation
This repository also contains the file `Window.cpp.diff` to remove the splash screen from EmulationStation (which normally can't be disabled by design [1]).

----
[1] https://github.com/Aloshi/EmulationStation/issues/203
