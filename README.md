# Linux-Driver-Based-Smart-Home-Control-System
Linux驱动智能家居控制系统
项目简介
基于Linux嵌入式平台开发的智能家居控制系统，上位机通过Qt界面控制硬件模块，下位机通过字符设备驱动管理ADC、超声波传感器、舵机和直流电机，实现实时监控与远程报警。

技术栈
C++ / Qt / Linux驱动 / TCP Socket / 设备树 / 字符设备

核心工作
驱动开发：编写Linux字符设备驱动，结合平台设备与设备树管理LED、蜂鸣器、ADC、超声波、舵机、直流电机

应用开发：Qt Widgets实现上位机控制界面，QTimer + MonitorThread实现传感器数据定时采集与实时显示

网络通信：TCP Socket实现上下位机数据交互，延迟＜100ms，异常自动报警

项目成果
系统实时显示光强、距离、舵机角度和马达状态，上位机可远程控制全部硬件模块。
