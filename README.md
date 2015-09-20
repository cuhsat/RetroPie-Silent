# RetroPie Silent
Basic configurations to silence all system outputs for RetroPie 3.0

Please execute the following command line to silence various outputs:
```
$ ./retropie_silent.sh
```

## System Outputs
This will turn off the following outputs

### [Raspian](https://www.raspbian.org)
* Boot logo
* Kernel messages
* Voltage warnings
* Temperature warnings
* Rainbow splashscreen

### [Libretro](http://www.libretro.com)
* OSD (On Screen Display)

### [EmulationStation](http://www.emulationstation.org)
* Loading messages

### [RetroPie](http://blog.petrockblock.com/retropie/)
* Splash screen (disables service)

## Additional Options
This will also set the following options
* Force sound over HDMI
* Turn off boot delay

## Additional Files
In case you want to disable the EmulationStation splash screen, please apply the `EmulationStation.diff` file to the source code before compiling it.

----
Have fun!
