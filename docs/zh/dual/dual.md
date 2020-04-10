# 单双色系列

仰邦单双色系列包括所有的五代与六代控制器。

其中五代控制器主要包括：

BX-5A/BX-5M/BX-5E以及 XW 系列控制器

而六代控制器主要包括：

BX-6A/BX-6M/BX-6E/BX-6Q 系列控制器

**注：六代控制器为五代控制器的升级版本，新的项目建议使用六代控制器。而对于五代控制器，由于其在市场上一直有广泛的使用，五代控制器我们也会持续长期供货。**

----



## 1. 开发前必读

### 1.1 关于动态区

**如果您的应用，需要对显示内容进行频繁刷新，请一定仔细阅读此章节!**

根据存储介质的不同，我们将控制器上现实的内容分为两类：普通节目（数据存储在flash中）和动态区（数据存储在ram中）。普通节目可以包括各种区域：时间区、传感器区、图文区等。

普通节目，会被存储在控制器的flash中，其内容掉电不丢失，但是因为flash存储器擦写寿命只有十万次，所以，其不能用于更新频率很高的场合，例如：停车场车位信息，外部传感器状态的实时更新，车次状态的实时更新等。

动态区完全独立于普通节目，其内容可以按区域进行单独更新，它可以与普通节目一起播放，也可以单独播放，它最大的特点是内容存储在ram中，没有擦写次数限制，内容掉电不保存，通常用于信息更新频繁场合。

而并非所有的控制器都支持动态区，目前支持动态区的控制器型号有：

BX-5E/BX-6E/BX-6Q 系列

### 1.2 网络通讯模式

针对网络通讯，我们的 SDK 提供了两种通讯模式：

**a. client 模式**

此种模式下，SDK 作为客户端，控制器作为服务端。此时，控制器的 IP 地址与端口固定，SDK主动发起与控制器的连接。此种模式通常应用于SDK与控制器处于同一局域网的场合。

**b. server 模式**

此种模式下，SDK 作为服务端，控制器作为客户端。SDK所在服务器的 IP 地址固定，控制器主动连接服务端，并主动维持此长连接。并且，控制器具备自动断后重连的机制。此种模式通常应用于广域网或者 GPRS/3G/4G 无线通讯的场合。

### 1.3 准备工作

在进行开发之前，请使用通用软件LedshowTW图文编辑软件对控制器进行相关配置，比如控制器IP地址（串口号）、屏幕参数、扫描方式等，在使用LedshowTW软件能发送普通节目到控制器兵能显示正常后，在进行二次开发。

---

## 2. 我们可以提供的开发包

对于五代/六代单双色控制器，我们可以提供以下开发包及其 Demo。

| #    | 语言                 | 操作系统                   |
| ---- | -------------------- | -------------------------- |
| 1    | [JAVA](../java/java) | Windows/Linux/Android/iMac |
| 2    | C++                  | Windows/Linux              |
| 3    | C#                   | Windows                    |
| 4    | VB                   | Windows                    |
| 5    | Delphi               | Windows                    |

> 注：针对不同的 linux 发行版，SDK 可能需要重新编译。此时，您可联系我们并获得支持。此时，可能需要您提供相应的编译工具链。

---
