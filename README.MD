
# update 20190922

Max30102的美信官方例程附带了计算心率血氧的基本算法，是一个不错的算法入门方案，但是其是C++编写的，并且带了个mbed的操作系统，而我一直用c编写stm32程序。因此一年前我花了一下午时间把美信官方例程移植为c版本的stm32裸机程序，随手放到了csdn上，没想到一年过去下载量还挺高，csdn也自动把下载所需的积分调整到高达23分（太不道德了，导致很多人下不了...），为了能让更多人下载，所以干脆放到github上。

# 下面写于一年前

MAX30102心率血氧显示例程，C语言，裸机代码。移植自美信官方例程。
最近需要用stm32做心率血氧测试，找了下要么是只有芯片驱动没有算法，要么是美信的官方例程，而官方例程是用C++写的，还跑了个叫mbed的操作系统......非常不爽，弄了一下午，移植成功，特地分享上来，觉得好的给个好评！

注意：
网上的PA2/PA3引脚为串口传输的都是美信官方例程！用C++写的，还带个mbed的操作系统。

- 供电3-5V
- MAX30102模块接口: PB9-SDA, PB8-SCL, PB7-INT, PA9/PA10是串口TX/RX
- 波特率: 115200


