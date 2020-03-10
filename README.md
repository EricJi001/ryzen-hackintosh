## AMD Ryzen Hackintosh 

### 配置

|   Component    |             Model              |
| :------------: | :----------------------------: |
|      CPU       | AMD Ryzen 5 1400 @ 3.8GHz (OC) |
|  Motherboard   |       ASUS PRIME B350M-A       |
|      RAM       |   8GB (2 x 4GB) A-DATA @2666   |
| Audio Chipset  |            ALC-887             |
|      GPU       | MSI GTX 1050Ti/Sapphire RX 460 |
| OS Disk (NVMe) |     Samsung 970 Pro 512GB      |

**macOS 版本**: 10.13.6 (17G11023)/10.14.6(18G3020)

**OpenCore 版本**: 0.5.5/0.5.6

## 说明

1.声卡注入ID为52

2.未测试麦克风是否可用

3.虚拟化相关软件不可用，因为是AMD CPU...

4.config文件并没有三码，请自行解决

5.显示器为4K，config文件中调整了开机屏幕显示缩放比例

6.没有无线网卡，有网卡的请自行解决config配置问题

7.未勾选showpicker选项，所以默认开机加载第一位置的系统，多系统请自行搜索相关设置

8.添加1050Ti原生电源管理

9.删除DSDT.aml 会造成windows 10无法启动

10.更新kext为最新

11.添加AMD-USB-Map.kext 定制PTXH控制器内的端口，请自行修改其他[参考链接](https://github.com/khronokernel/Opencore-Vanilla-Desktop-Guide/blob/master/AMD/AMD-USB-map.md)

12.添加AMD CPU的温度检测插件SMCAMDProcessor.kext，基于VirtualSMC.kext，可[参考链接](https://github.com/trulyspinach/SMCAMDProcessor)

...

