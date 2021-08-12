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

## Fix issues
  - Serial number/mac address ... [here](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#using-gensmbios){:target="_blank"}.
  - WiFi : 
    - Use external USB WiFi -> Wirless USB Adapter above.
    - Use internal WiFi -> [here](https://openintelwireless.github.io/itlwm/Installation.html#itlwm){:target="_blank"}.
  - Sleep -> [here](https://dortania.github.io/OpenCore-Post-Install/universal/sleep.html#preparations){:target="_blank"}.
      - ActivateHpetSupport = true in Config.plist (UEFI tab).
      - [Recommended](https://dortania.github.io/OpenCore-Post-Install/usb/misc/keyboard.html#method-3-configuring-darkwake){:target="_blank"}.
      - Turn off (Wake for Ethernet Network access and Enable Power Nap) in Enegy saver settings. And ```sudo pmset -a standby 0``` [here](https://hackintosher.com/forums/thread/improving-sleep-on-a-hackintosh-wakeup-freezes-black-screens.486/){:target="_blank"}.
      - [Coffee Lake systems failing to wake](https://dortania.github.io/OpenCore-Install-Guide/troubleshooting/extended/post-issues.html#coffee-lake-systems-failing-to-wake){:target="_blank"}.
      - [Optional](https://dortania.github.io/OpenCore-Post-Install/usb/misc/instant-wake.html){:target="_blank"}.
  - Video how to patch PCI devices to correct Device Properties in Config.plist
      - [Sample fix wifi on Big Sur](https://www.youtube.com/watch?v=bp06YxnKNTk){:target="_blank"}.
      - [Show Config.plist](https://www.youtube.com/watch?v=BAGp_QfFGf4){:target="_blank"}.
  ## Others
  - [Link](https://www.hackintosh-forum.de/forum/thread/53016-dell-latitude-5490/){target="_blank"}.
  - [Tool check OpenCore](https://opencore.slowgeek.com/){:target="_blank" rel="noopener"}.
  - <a href="http://example.com/" target="_blank">Test link</a>
  - %md <a href="https://google.com" target="_blank">google link</a>
  - <a href="https://google.com" target="_blank" rel="noopener">external link</a>