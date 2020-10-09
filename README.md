# macOS-10.15.7-OC-0.6.3-XPS-7590-IPS-4K-Touch
My working EFI for the Dell XPS 7590 with a 4K IPS touch screen!

Please note this EFI is based off: https://github.com/romancin/Dell-XPS-7590-OpenCore

I have updated some kexts, and made some light SSDT edits to enable the touch screen and update OC to 0.6.3.
This EFI Has been tested on 10.15.7 and testing on Big Sur Beta's will be going on soon. I will report as I go.

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

# Things That Work:
⋅⋅*TOUCHSCREEN 4K Display w/ Scaling
⋅⋅*Full 2GB Graphics Acceleration
⋅⋅*Sound / Headphone port / HDMI audio out / Mic In
⋅⋅*ALL USB / USB-C ports
⋅⋅*Sleep / Close-Lid & re-open
⋅⋅*Bluetooth and Wifi (with card seen above)
⋅⋅*Power Management (I get about 4 hours) -> I am still working on undervolting

# Not Working Items:
⋅⋅*Stock BT / WIFI
⋅⋅*Nvidia 1650 dGPU
⋅⋅*SD Card Reader

# Overall:
Overall this thing is a beast and dual-boots Windows 10 like a champ. 
