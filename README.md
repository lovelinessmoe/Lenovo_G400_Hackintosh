# Lenovo_G400_Hackintosh
基于https://github.com/autersu/Lenovo_G400_EFI
联想G400 10.15.7黑苹果

## 机型以及配置说明

* 电脑型号	联想 Lenovo G400 20235 笔记本电脑 

* 处理器	英特尔 第三代酷睿 i5-3230M @ 2.60GHz 双核 四线程 ivy Bridge架构

* 主板	联想 00000000Not Defined ( Intel HM76 Express 芯片组 )

* 内存	8 GB+4 GB ( 镁光 DDR3L 1600MHz / 记忆科技 DDR3L 1600MHz )

* 主硬盘	海康威视 C160 256G SSD

* 集成显卡	Intel(R) HD Graphics 4000

* 核心显卡	AMD Radeon HD 8570M  (2G显存) 

* 显示器: 奇美 CMO1461 (14 英寸)

* 声卡	Conexant SmartAudio HD @ 英特尔 Panther Point High Definition Audio Controller

* 有线网卡	鈺硕 QCA8172 Fast Ethernet / 联想

* 无线网卡	Intel(R) Centrino(R) Wireless-N 135 BGN

* 蓝牙	Qualcomn Atheros AR3012 Bluetooth 4.0


## 已经实现功能

1. 声卡

2. 显卡

3. 蓝牙

4. 键盘+触摸板(手势不好用，太小了)

5. 有线网卡

6. 无线网卡

7. USB定制

8. 摄像头

## 无法实现

1. 睡眠未测试，有可能出现睡死的情况

## KEXT
| KEXT                        | 说明                  | 必备 | 可选 |
| --------------------------- | --------------------- | ---- | ---- |
| ApplePS2SmartTouchPad.kext  | 触摸板和键盘            |  √   |      |
| AtherosE2200Ethernet.kext   | 有线网卡驱动            |      |   √  |
| CPUFriend.kext              | CPU管理。              |  √   |      |
| FakePCIID_XHCIMux.kext      | 1E31蓝牙USB控制器       |      | √    |
| FakePCIID.kext              | 上依赖                 |      | √    |
| HibernationFixup.kext       | 修复睡眠               | √    |      |
| IntelBluetoothFirmware.kext | 蓝牙框架               | √    |      |
| IntelBluetoothInjector.kext | 蓝牙驱动               | √    |      |
| itlwm.kext                  | 无线网卡驱动            |      |   √  |
| Lilu.kext                   | 驱动扩展库(超重要)      | √    |      |
| SMCBatteryManager.kext      | SMC电池                | √    |      |
| SMCProcessor.kext           | SMC处理器              | √    |      |
| SMCSuperIO.kext             | SMC风扇                | √    |      |
| USBPorts.kext               | USB定制                | √    |      |
| VirtualSMC.kext             | SMC(超重要)            | √    |      |
| VoodooHDA.kext              | 声卡驱动               |      |   √  |
| WhateverGreen.kext          | 核显驱动               | √    |      |


## 鸣谢
- [Apple](https://www.apple.com) 开发的 [macOS](https://www.apple.com/macos)
- [zxystd](https://github.com/zxystd) 开发的 [itlwm](https://github.com/OpenIntelWireless/zxystd)
- [Bat.bat](https://github.com/williambj1) 开发的 [IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware) 和 [HeliPort](https://github.com/OpenIntelWireless/HeliPort)
- [acidanthera](https://github.com/acidanthera) 开发的 [Lilu](https://github.com/acidanthera/Lilu) 和 [VirtualSMC](https://github.com/acidanthera/VirtualSMC) 和 [WhateverGreen](https://github.com/acidanthera/WhateverGreen) 
- [VoodooHDA](https://sourceforge.net/projects/voodoohda/)
