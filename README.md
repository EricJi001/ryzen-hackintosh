## AMD Ryzen Hackintosh 

### 配置

|   Component    |             Model              |
| :------------: | :----------------------------: |
|      CPU       | AMD Ryzen 5 1400 @ 3.8GHz (OC) |
|  Motherboard   |       ASUS PRIME B350M-A       |
|      RAM       |   8GB (2 x 4GB) A-DATA @2666   |
| Audio Chipset  |            ALC-887             |
|      GPU       |         MSI GTX 1050Ti         |
| OS Disk (NVMe) |     Samsung 970 Pro 512GB      |

**macOS 版本**: 10.13.6 (17C8037)
**OpenCore 版本**: 0.5.4

## 说明

1.声卡注入ID为52

2.未测试麦克风是否可用

3.虚拟化相关软件不可用，因为是AMD CPU...

4.config文件并没有三码，请自行解决

5.显示器为4K，config文件中调整了开机屏幕显示缩放比例

6.没有无线网卡，有网卡的请自行解决config配置问题

7.未勾选showpick选项，所以默认开机加载第一位置的系统，多系统请自行搜索相关设置

...