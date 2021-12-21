# ibox4.0_remote_host_controller
Ruetz Testerlyzer I-Box 4.0 Remote Control via host PC

Pre-requisites:

- Ruetz-Ibox 4.0 with HCS ( Host Control Support) enabled;
- Python with modules - pyserial and argparse;
- USB type B (Testerlyzer I-Box 4.0) to USB type A (Host device)

This simple Python script controls the frontal clamps (CL30, CL30f, CL30b, Mute and OBD buttons) of the Testerlyzer I-box 4.0 power supply.

https://ruetz.de/en/testing/products/index.php

![Image description](https://i.imgur.com/gz6GAd7.png)

Usage:
```
$ python ibox_remote_HCS.py -h
usage: ibox_remote_HCS.py [-h] -p PORT [--check_clamps] [--check_firmware] [--start_clamps] [--shutdown_clamps] [--turn_on {cl30,cl30f,cl30b,mute,obd}] [--turn_off {cl30,cl30f,cl30b,mute,obd}] [--restart {cl30,cl30f,cl30b,mute,obd}]
 
Ruetz Ibox Host PC Controller
 
optional arguments:
  -h, --help            show this help message and exit
  -p PORT, --port PORT  Specify serial port
  --check_clamps        Check all clamp status
  --check_firmware      Check firmware version
  --start_clamps        Start all power clamps (cl30,cl30f,cl30b)
  --shutdown_clamps     Shutdown all power clamps (cl30,cl30f,cl30b)
  --turn_on {cl30,cl30f,cl30b,mute,obd}
                        Turn on clamp cl30/cl30f/cl30b/mute/obd
  --turn_off {cl30,cl30f,cl30b,mute,obd}
                        Turn off clamp cl30/cl30f/cl30b/mute/obd
  --restart {cl30,cl30f,cl30b,mute,obd}
                        Restart clamp cl30/cl30f/cl30b/mute/obd
  ```
