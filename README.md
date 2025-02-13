# HAControlCLI
[![Xun-X](https://img.shields.io/static/v1?label=作者&message=Xun-X&color=F36CB0)](https://github.com/Xun-X/HAControlCLI)
[![Xun-X](https://img.shields.io/static/v1?label=特别感谢&message=HomeAssistant&color=97C40F)]([https://nezha.wiki/](https://www.home-assistant.io/))
[![Xun-X](https://img.shields.io/static/v1?label=软件特点&message=简单、易用&color=48C21A)](https://github.com/Xun-X/HAControlCLI)
[![Xun-X](https://img.shields.io/static/v1?label=软件性质&message=免费、非开源&color=1081C2)](https://github.com/Xun-X/HAControlCLI)
[![Xun-X](https://img.shields.io/static/v1?label=获取方式&message=Github下载&color=F48041)](https://github.com/Xun-X/HAControlCLI)

Windows 快速控制 Home Assistant 设备开启或关闭

# 功能说明
极致简单的一个快速控制 Home Assistant 里添加的设备的开启或关闭

# 使用方法
1、下载 HAControlCLI.exe 程序

2、首次直接双击运行，弹出配置界面，会在运行目录下创建[HAControlCLI.hadb]文件，里面保存API和服务器地址

3、按照下方 [使用方法] 使用即可

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

## 方法1：
Windows 操作系统 按下 Win键 + R 启动[运行]窗口，按照如下格式的内容运行即可

开启 "D:\HAControlCLI.exe 1 实体标识符" 

关闭 "D:\HAControlCLI.exe 0 实体标识符"

## 方法2：
1.HAControlCLI.exe 所在目录创建2个文件，分别是“on.bat”和“off.bat”

2.用记事本打开“on.bat”，输入如下内容：
```
HAControlCLI.exe 1 实体标识符
```

3.用记事本打开“off.bat”，输入如下内容：
```
HAControlCLI.exe 0 实体标识符
```
4.运行“on.bat”就会开启设备的开关 / 运行“off.bat”就会关闭设备的开关

没有技术难度的小工具，就是通过post请求，控制设备开启或关闭的简单程序

# 下载地址
[点击下载](https://raw.githubusercontent.com/Xun-X/HAControlCLI/refs/heads/main/HAControlCLI.exe "点击下载")

# 使用注意
需自行搭建好 Home Assistant 平台，添加好自己的智能开关等设备

(Home Assistant在Youtube有视频教程，安装部署很简单)
