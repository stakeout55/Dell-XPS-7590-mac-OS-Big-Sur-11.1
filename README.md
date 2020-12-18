# Dell XPS 7590 macOS Big Sur 11.1
My working EFI for the Dell XPS 7590 with a 4K IPS touch screen!

#### Updated 12-17-2020

### YOU MUST ADD YOUR OWN INFO UNDER PLATFORM INFO!!!
---

## Sources that this EFI is based off of: 
https://github.com/romancin/Dell-XPS-7590-OpenCore

https://github.com/xxxzc/xps15-9570-macos

https://dortania.github.io/OpenCore-Install-Guide/

https://github.com/jaromeyer/XPS9570-Catalina

---

Shout out to [u/Zero00Shadow](https://www.reddit.com/user/Zero00Shadow) for his extensive testing for performance and battery, etc - results coming soon

I have updated some kexts, and made some light SSDT edits to enable the touch screen and update OC to 0.6.3.
This EFI Has been tested on 10.15.7 and testing on Big Sur Beta's will be going on soon. I will report as I go.

---

The build of my laptop is as follows:
| First Header  | Second Header |
| ------------- | ------------- |
| CPU:   | Intel Core i7 9750H  |
| iGPU:   | Intel Graphics UHD 630  |
| dGPU:  | Nvidia GeForce GTX 1650  |
| Screen:  | IPS 4K Display (non OLED)  |
| Ram:  | Stock 16gb  |
| SSD:  | Stock 500gb NVME  |
| WiFi/BT: | [M.2 BCM94360NG (native)](https://www.ebay.com/itm/M-2-NGFF-Network-Card-for-Broadcom-BCM94360NG-better-than-BCM94352Z-DW1560-BT4-0/264663343680?ssPageName=STRK%3AMEBIDX%3AIT&_trksid=p2057872.m2749.l2649) |

---

# Things That Work:
* TOUCHSCREEN 4K Display w/ Scaling
* Full 2GB Graphics Acceleration
* Sound / Headphone port / HDMI audio out / Mic In
* ALL USB / USB-C ports
* Sleep / Close-Lid & re-open
* Bluetooth and Wifi (with card seen above)
* Power Management
* SD Card Reader

---

# Not Working Items:
* Stock BT / WIFI
* Nvidia 1650 dGPU

---
# Buggy at times:
* HDMI hot plugging. Sometimes upon disconnect the laptop thinks that it still has two displays to work with when it doesn't. Simply close the lid and reopen to fix.

---

# Overall:
Overall this thing is a beast and dual-boots Windows 10 like a champ. 
