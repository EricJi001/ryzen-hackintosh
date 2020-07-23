AMD Ryzen Hackintosh 

### 配置

|   Component    |             Model              |
| :------------: | :----------------------------: |
|      CPU       | AMD Ryzen 5 1400 @ 3.7GHz (OC) |
|  Motherboard   |       ASUS PRIME B350M-A       |
|      RAM       |   8GB (2 x 4GB) A-DATA @2666   |
| Audio Chipset  |            ALC-887             |
|      GPU       | MSI GTX 1050Ti/Sapphire RX 460 |
| OS Disk (NVMe) |     Samsung 970 Pro 512GB      |

**macOS version**: 10.13.6 (17G11023)/10.14.6(18G4032)/10.15.6 (19G73)

**OpenCore version**: 0.5.5/0.5.7/0.5.9

## Tips：

1.LayoutID = 50

2.No test microphone

3.The virtual machine application is not available

4.config.plist does not contain Serial/Board Serial/SmUUID number

5.The display resolution is 4k, so UIScale = 02

6.No WiFi chipset

7.Default OS is macOS, if you used win10 + macOS

8.Add 1050Ti PM

9.Update kext  

10.Add AMD CPU temperature plug-in: SMCAMDProcessor.kext，this kext based on VirtualSMC.kext，see [this link](https://github.com/trulyspinach/SMCAMDProcessor)

...

