# wlanpi-nanohat-oled-scripts

*Collection of scripts to provide features for wlanpi-nanohat-oled menu options*

This is a collection of control scripts used by the front panel menu system detailed in the WLANPi project : [wlanpi-nanohat-oled](https://github.com/WLAN-Pi/wlanpi-nanohat-oled). Each script is used to start, stop and display the status of a specific process that is being controlled by the front panel menu.

Each of these bash scripts interact with a different Linux application/process to enable it to be controlled by the front panel menu system.

Each script is very simple, providing a start, stop and status function. The output from each script is a short text message to indicate the process status that may be used in the front panel menu system.

## Scripts

The following scripts are supported to date. Each has its own information page which is linked below:

 - kismet_ctl (https://github.com/WLAN-Pi/wlanpi-nanohat-oled-scripts/doc/kismet_ctl.md
 - bettercap_ctl (https://github.com/WLAN-Pi/wlanpi-nanohat-oled-scripts/doc/bettercap_ctl.md 
 
Note that a minimum version of [wlanpi-nanohat-oled.py](https://github.com/WLAN-Pi/wlanpi-nanohat-oled) v0.20 or later is required to use these controls

## Installation

To install the scripts, obtain the gzipped archive file in the "bundle" directory of the project github repo (https://github.com/WLAN-Pi/wlanpi-nanohat-oled-scripts/bundle)

Log in to the WLANPi as the "wlanpi" user. Copy the archive file into the /home/wlanpi directory of the WLANPI. Extract the files from the archive using the commands:

```
 # Note this operation is done as the WLANPi user
 cd /home/wlanpi
 tar xvfz wlanpi-nanohat-oled-scripts-v0.01.tar.gz
```
 
Installation is now complete. The WLANPi front panel menu system (ver 0.20 or later) will now be able to check the status, start or stop each of the processes controller by the scripts. (See the options available under the front panel menu option Home -> 3.Actions )
