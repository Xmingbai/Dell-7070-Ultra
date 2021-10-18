# Dell-7070-Ultra

![](https://github.com/Xmingbai/Dell-7070-Ultra/blob/main/%E6%88%AA%E5%B1%8F2021-10-18%20%E4%B8%8B%E5%8D%8810.37.00.png)



要想流畅体验macOS操作系统，必须修改bios 

# 以下重要BIOS设置选项，需关闭
安全启动
SGX
TPM 

硬件配置：
CPU： i7-8565U
内存： 2根8G DDR4 2400
硬盘：东芝2242 NVME SSD 512G+ SATA SSD 1T
WIFI：BCM94352Z

# 还需要使用Grub 命令行工具修改以下参数

必选：修改dvmt对应值为64M   对应命令  setup_var    0xA13   0x2  （不修改核显驱动不正常）

可选 ：解锁cfg lock 为disable  对应命令    setup_var  0x6F0   0x0  

OC引导目前驱动完善程度 接近白果

成功安装macOS11.6 理论支持12.x

目前驱动情况
关于本机基本信息识别正

CPU 核心数   睿频正常

有线网卡驱动正常

板载无线9565AC 更换为BCM94352Z，无线 wifi及蓝牙正常，支持隔空投送随航

3.5音频 、TYPE-C音频及显示器音频都正常

这里有一个tips，Dell很多机型包括这台7070，必须搭配HPET补丁才能识别到声卡

核显驱动正常 4K视频预览流畅

睡眠唤醒皆正常

macOS完美程度非常接近白果
