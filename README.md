# HP-15-ax015TX-MAC10.15.4-OC-EFI
## 惠普暗影精灵2-15-ax015TX  
| 硬件| 型号|   
| :----: | :----: |
| CPU | I5 6300HQ |    
|内存 | 8G*2 DDR4 |     
|显卡| Intel HD Graphics 530 + NVIDIA GeForce GTX 960Mi |     
|网卡| Realtek RTL8111H + BCM94352z |     
|声卡| Realtek ALC295  |   
## 系统支持
系统：macOS 10.15.6 b2  
EFI:0C6.0  
### 正常功能：  
1. 显卡
2. FN按键
3. 电源管理
4. 睡眠
5. 声音
6. 蓝牙
7. 触摸板
8. 摄像头

### 进展
#### CPU变频：  
已启用 X86 原生电源管理，将闲时频率从 1.2GHz 降低到 0.8GHz，并更改 EPP 为节能模式（0x80）
睡眠和唤醒：支持合盖睡眠和唤醒，支持 USB 设备唤醒（当使用电池进行睡眠时，所有外置设备将自动断电无法进行唤醒）。
#### 声卡  
取至 XStar-Dev（https://github.com/XStar-Dev/）：
自编译 AppleALC，基于黑果小兵 ALC295 的 layout-id=13 修改，已重新定制相关的布局文件，修复热启动时 CPU 占用过高问题

