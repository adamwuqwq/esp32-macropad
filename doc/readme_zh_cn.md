# 一个低成本小型宏键盘
## 综述

## 我的idea（硬件架构）
由于最近非国产MCU（例如Atmega328）大幅涨价，在此项目中便采用便宜大碗还支持2.4G WiFi的ESP8266作为主控制器。  
在这个项目中，由于GPIO接口数量有限，我们将采用矩阵键盘的形式，共5*5=25个按键，仅需要占用5+5=10个IO接口。在按键HID模拟方面，我采用了便宜且不需要很多外围元件的CH9329方案，通过串口UART与MCU通信。其中OLED屏用来显示状态（例如正在按下的按键），采用I2C总线与MCU通信。  

## 使用的零件
ESP8266模块 1个  
白色OLED屏幕 1个  
轴体 25个  
CH9329芯片 1个  
CH340G芯片 1个  
贴片电阻电容连接器LED等 若干（参考BOM清单）  

## 键盘的布局设计
考虑到用途，本键盘模仿标准104键键盘的小键盘，共设有25个按键，布局如下图：  

## 实现的功能
计划实现：
可以自定义映射的宏建盘  
5组内置keymap预设，可切换  
Qt编写的上位机软件，图形化编辑keymap  
通过Wifi热点连接，在网页上编辑keymap  
通过按键来HID模拟鼠标  
支持固件升级  
未实现：  
更换主控为ESP32，增加电池，实现蓝牙连接  
-因成本过高，且没有相关需求，暂时搁置  

## PCB绘制

## 参考资料
KiCAD keyboard PCB design guide  
https://deskthority.net/wiki/KiCAD_keyboard_PCB_design_guide  
Keyboard PCB guide  
https://github.com/ruiqimao/keyboard-pcb-guide/blob/ddf843ee5a5d36edd875370d22974dc7cd6f62e4/README.md  
KiCadで雑に基板を作る チュートリアル  
https://www.slideshare.net/soburi/kicad-53622272  
MIT License
