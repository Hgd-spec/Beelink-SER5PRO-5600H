# Beelink-SER5PRO-5600H
零刻ser5pro-5600H黑苹果EFI（wifi无法驱动）

- 系统版本：macOS Sonoma 14.1 (23B74)
- 网卡：ax200
- 硬盘：京造5系 512g
- 内存：杂牌ddr4 3200
- CPU：5600H
- 显卡：核显

蓝牙、网线、声卡等可以正常使用，暂时知道的是wifi不能用
也尝试过ventura、High_Sierra都是wifi不能用
本人小白，现学现卖

## 找到问题所在了，基本无解
macos没初始化这个网卡设备，acpi没生成中断，pcie寄存器也全是脏的。（感谢zxystd大神解答）

### 基于[@Xmingbai](https://github.com/Xmingbai)和[@daliansky](https://github.com/daliansky)两位大神提供的EFI修改,感谢！
