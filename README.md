# HAControlCLI
快速控制 Home Assistant 设备开启或关闭

# 功能说明
极致简单的一个快速控制 Home Assistant 里添加的设备的开启或关闭

# 使用方法
下载 HAControlCLI.exe 程序，双击运行，弹出配置界面

# 首次配置方法：
如图：

![](https://raw.githubusercontent.com/Xun-X/HAControlCLI/refs/heads/main/images/1.png)

1、界面中填入 Home Assistant 的[WEB访问地址]，注意结尾不加“/”
例如：“http://192.168.1.123:8123”

2、界面中填入在 Home Assistant 里创建的[长期访问令牌]

# 使用方法：
通过运行命令快速开启/关闭设备
第一个参数 开或关。即：1=开 0=关
第二个参数 实体标识符。Home Assistant里找到对应设备开或关的 "实体标识符"
例如：
开启 "D:\HAControlCLI.exe 1 实体标识符"
关闭 "D:\HAControlCLI.exe 0 实体标识符"

没有技术难度的东西，就是通过post请求设备开启或关闭的简单程序
