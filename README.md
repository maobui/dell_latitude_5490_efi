# Dell Latitude 5490 EFI

# Clover
## Support for macOs versions:
  - Version 10.13: "High Sierra"
  - Version 10.14: "Mojave"
  - Version 10.15: "Catalina"
 
  Everything works except WiFi (use external usb wifi instead of and use [Wireless USB Adapter](https://github.com/chris1111/Wireless-USB-Adapter)).

## Optional
  Clover for Dell latitude 5590.

## Others
- [Link](https://osxlatitude.com/forums/topic/8506-dell-latitude-inspiron-precision-vostro-xps-clover-guide)
- [MacEFI](https://macefi.com/)


# OpenCore

## Support for macOs versions:
 - Version 11: "Big Sur"

## Build Config.plist
 - [Link](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html)
## Fix issues
  - Serial number/mac address ... [here](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#using-gensmbios).
  - WiFi : 
    - Use external USB WiFi -> Wirless USB Adapter above.
    - Use internal WiFi -> [here](https://openintelwireless.github.io/itlwm/Installation.html#itlwm).
  - Sleep -> [here](https://dortania.github.io/OpenCore-Post-Install/universal/sleep.html#preparations).
      - [Recommended](https://dortania.github.io/OpenCore-Post-Install/usb/misc/keyboard.html#method-3-configuring-darkwake).
      - Turn off (Wake for Ethernet Network access and Enable Power Nap) in Enegy saver settings. And ```sudo pmset -a standby 0``` [here](https://hackintosher.com/forums/thread/improving-sleep-on-a-hackintosh-wakeup-freezes-black-screens.486/).
      - [Coffee Lake systems failing to wake](https://dortania.github.io/OpenCore-Install-Guide/troubleshooting/extended/post-issues.html#coffee-lake-systems-failing-to-wake).
      - [Optional](https://dortania.github.io/OpenCore-Post-Install/usb/misc/instant-wake.html).
  - Video how to patch PCI devices to correct Device Properties in Config.plist
      - [Sample fix wifi on Big Sur](https://www.youtube.com/watch?v=bp06YxnKNTk).
      - [Show Config.plist](https://www.youtube.com/watch?v=BAGp_QfFGf4).
  - Cannot update to newer versions of Big Sur
      - [Link](https://dortania.github.io/OpenCore-Install-Guide/extras/big-sur/#cannot-update-to-newer-versions-of-big-sur).
  - Cannot upgrade OS:
      - Enable csr-active-config for upgrade only, after upgrade -> disbale it.
      - [Link](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html#nvram).
  ## Others
  - [Link](https://www.hackintosh-forum.de/forum/thread/53016-dell-latitude-5490/).
  - [Tool check OpenCore](https://opencore.slowgeek.com/).

# System information

## Configuration

| Specifications      | Details                                          |
| :---                |:---                                              |
| Computer model      | Dell Latitude 5490                               |
| Processor           | Intel Core i5-8350U Processor @ 1.8 GHz          |
| Memory              | 16 GB DDR4 2400 MHz                              |
| Hard Disk           | SSD 256                                          |
| Integrated Graphics | Intel(R) UHD Graphics 620                        |
| Screen              | Display @ 1920 x 1080 (13.9 inch)                |
| Sound Card          | Realtek ALC256                                   |
| Wireless Card       | Intel Dual Band Wireless-AC 8265/8275            |
| Bluetooth Card      | Intel Bluetooth 8265/8275                        |

  # Screens

  ![System Overview](./images/sys.png)

  ![System Preferences](./images/sys_pref.png)

  ![Sytems Bar](./images/sys_bar.png)

  ![Bluetooth](./images/bluetooth.png)

  ![Graphics](./images/graphics.png)

  ![Wifi](./images/wifi.png)
  