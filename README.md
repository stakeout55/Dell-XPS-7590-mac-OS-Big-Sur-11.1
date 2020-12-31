# Dell XPS 7590 macOS Big Sur 11.1
My working EFI for the Dell XPS 7590 with a 4K IPS touch screen!

See [latest release](https://github.com/stakeout55/Dell-XPS-7590-mac-OS-Big-Sur-11.1/releases/latest) for the latest EFI release

---

## Sources that this EFI is based off of: 
* This being my primary: 
  * https://github.com/xxxzc/xps15-9570-macos
* https://github.com/romancin/Dell-XPS-7590-OpenCore
* https://github.com/xxxzc/xps15-9570-macos
* https://dortania.github.io/OpenCore-Install-Guide/
* https://github.com/jaromeyer/XPS9570-Catalina
* https://github.com/CryptoNeverSleeps/XPS15-7590-Hackintosh
* https://github.com/daliansky/XPS15-7590-Hackintosh
* https://github.com/gorquan/OC-XPS-7590

---

Shout out to [u/Zero00Shadow](https://www.reddit.com/user/Zero00Shadow) for his extensive testing for performance and battery, etc - results coming soon

I have updated some kexts, and made some light SSDT edits to enable the touch screen and update OC to 0.6.4.
This EFI Has been tested on 10.15.5 - 11.1. I will update/report as I go.

---

The build of my laptop is as follows:
| Part          | Name |
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
* Sound / Headphone port / / Mic In
* ALL USB / USB-C ports
* Webcam
* Sleep / Close-Lid & re-open
* Bluetooth and Wifi (with card seen above)
* Power Management
* SD Card Reader (slow speeds but it works)
* Handoff
* Continuity
* AirDrop
* HDMI out + audio (read below for hot plug issue)

---

# Not Working Items:
* Stock BT / WIFI --> could use [OpenIntelWireless kext](https://github.com/OpenIntelWireless/itlwm) but likely won't have ability to get iServices working
* Nvidia 1650 dGPU
* Finger print reader (likely never will)

---
# Buggy at times:
* HDMI hot plugging. Sometimes upon disconnect the laptop thinks that it still has two displays to work with when it doesn't. Simply close the lid and reopen to fix.

---

## Tweaks for better performance:

* More natural trackpad: _System Preferences > Trackpad > "Turn off Force Click and haptic Feedback"_
  * Coutersey of [u/Zero00Shadow](https://www.reddit.com/user/Zero00Shadow) *
 
* UnderVolting with this modified/pre-signed kext: see my repo [here](https://github.com/stakeout55/presigned_VoltageShift_Kext_DellXPS7590). Details for the clocks are found on that repo too + how to use.

* WIP taping / thermal pads for better thermal performance... have some sources found here that I and [CryptoNeverSleeps](https://github.com/CryptoNeverSleeps) are testing:
   * https://www.reddit.com/r/Dell/comments/6gnfbv/easy_massive_thermal_improvements_on_dell_xps_13/
   * https://www.reddit.com/r/Dell/comments/cua4jl/dell_xps_7590_where_should_i_place_thermal_pad/
   * https://www.reddit.com/r/Dell/comments/jj26fz/taping_fins_mod_and_temp_differences_xps_15_7590/
   * http://forum.notebookreview.com/threads/cpu-gpu-temperatures-benchmarks-xps-15-9560-kaby-lake.802345/
    * These methods feature [thermal pads](https://www.amazon.com/ARCTIC-Thermal-Efficient-Conductivity-Handling/dp/B00UYTTMNI?th=1) and/or [tape](https://www.amazon.com/Aluminum-Professional-Adhesive-3-9mil-1-Roll/dp/B08CXBPWNT/ref=sr_1_2_sspa?dchild=1&keywords=foil%2Btape%2Bheat%2Bsmall&qid=1609362425&sr=8-2-spons&smid=AEZRIMTHROAA2&spLa=ZW5jcnlwdGVkUXVhbGlmaWVyPUEyUDUxRFJUU0FMRjFKJmVuY3J5cHRlZElkPUExMDM4ODY5S1g0N1JOVFc4WkxCJmVuY3J5cHRlZEFkSWQ9QTAyNDE1MjBLTU9ZWE5GVzUzOTQmd2lkZ2V0TmFtZT1zcF9hdGYmYWN0aW9uPWNsaWNrUmVkaXJlY3QmZG9Ob3RMb2dDbGljaz10cnVl&th=1) of which we will be trying a mixture.

* Sleep testing "study" that was conducted revealed only a 14% drop in battery over the course of 19 hours (would have been less without as many "check-ins"):
![image]


# Overall:
Overall this thing is a beast and dual-boots Windows 10 like a champ. 
