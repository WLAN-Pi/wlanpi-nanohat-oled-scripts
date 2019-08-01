# WLANPi Kismet Control Script
*Shell script to enable/disable Kismet for the WLANPi*

This package is controlled using the menu system detailed in the WLANPi project : [wlanpi-nanohat-oled](https://github.com/WLAN-Pi/wlanpi-nanohat-oled)

## Requirements

To be able to start/stop Kismet on the WLANPi via the front panel menu, you will need:

 - Kismet on a WLANPi (installed as part of the std WLANPi distribution)
 - WLANPi distribution v1.7.2 or later installed on a WLANPi (https://github.com/WLAN-Pi/wlanpi/releases), which includes [wlanpi-nanohat-oled.py](https://github.com/WLAN-Pi/wlanpi-nanohat-oled) v0.20 or later

## Installation

To install the script, obtain the gzipped archive file in the "bundle" directory of the project github repo (https://github.com/WLAN-Pi/wlanpi-nanohat-oled-scripts/bundle)

Log in to the WLANPi as the "wlanpi" user. Copy the archive file into the /home/wlanpi directory of the WLANPI. Extract the files from the archive using the commands:

```
 # Note this operation is done as the WLANPi user
 cd /home/wlanpi
 tar xvfz wlanpi-nanohat-oled-scripts-v0.01.tar.gz
```

## Usage

The CLI usage instructions are shown below. These are not generally required, as this batch file is called by the WLANPi menu system. Each command returns a short textual status message to indicate the result of the attempted operation.

```
 cd home/wlanpi/nanohat-oled-scripts/
 
 # check Kismet status
 ./kismet_ctl status

 # Start Kismet
 ./kismet_ctl start

 # Stop Kismet
 ./kismet_ctl stop
```

