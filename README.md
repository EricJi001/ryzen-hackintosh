AMD Ryzen Hackintosh 

|   Component    |             Model              |
| :------------: | :----------------------------: |
|      CPU       | AMD Ryzen 5 1400 @ 3.7GHz (OC) |
|  Motherboard   |       ASUS PRIME B350M-A       |
|      RAM       |   8GB (2 x 4GB) A-DATA @2666   |
| Audio Chipset  |            ALC-887             |
|      GPU       |        Sapphire RX 460         |
| OS Disk (NVMe) |     Samsung 970 Pro 512GB      |
|      WiFi      |          Intel ax200           |

**macOS version**: 10.15.7 (19H15)/11.0.1 (20B29)

**OpenCore version**: 0.6.3

## Tips：

1.LayoutID = 50

2.No test microphone

3.The virtual machine application is not available

4.config.plist does not contain Serial/Board Serial/SmUUID number

5.The display resolution is 4k, so UIScale = 02

6.Add WiFi chipset, so added three kexts: AirportItlwm.kext, IntelBluetoothFirmware.kext and IntelBluetoothInjector.kext. WiFi kext repository is [Here](https://github.com/OpenIntelWireless/itlwm), you can find how to use it. 

These kexts only can drive Intel ax200，if you don't hava this chipset, you will need to modify the contents of the config.plist file, Path: Kernel/Add. 

Or if you have other intel WiFi chipset like AC9560, you can read [Here](https://docs.oiw.workers.dev/itlwm/), and must remove these three kexts, download again, because I modified these three kexts info.plist file.

P.S: this WiFi chipset speed is very slow, because Kext is  very new.

7.Default OS is macOS, ShowPicker is False.

8.Update kext  

9.Add AMD CPU temperature plug-in: SMCAMDProcessor.kext，this kext based on VirtualSMC.kext，see [this link](https://github.com/trulyspinach/SMCAMDProcessor)

...

