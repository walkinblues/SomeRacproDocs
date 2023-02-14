# 线上培训__声卡和Teams设置

**此文档是为了将本地电脑的音频和Mic同时投放到Teams,让线上的人听得到 **

**无需播放电脑声音的培训可以点关闭了 **

**太长不想看请按图设置**

---

Teams、声卡和Loopback软件的设置, 用于本地培训并且在线上会议直播的情况

以MacBook 、Microsoft Teams、  [Steinburg UR22C](https://www.steinberg-cn.com/audio-interfaces/ur22c/)、[Rogue Amoeba | Loopback](https://rogueamoeba.com/loopback/)为示例

loopback是为了将本地电脑的音频投放到Teams, 无此需求的培训只需要将Mic信号送到Teams(不使用loopback功能)

有loopback功能的声卡, 则无需Rogue Amoeba Loopback这类软件, 在声卡内部设置即可

## 声卡

声卡的物理输入接口作为Mic输入, 物理输出给到本地功放音箱

## 电脑音频输出

音频输出选择Loopback Audio, 即送到Loopback软件里的Pass-Thru

<img src="./OnlineTrainin_TeamsSoundCardSettings_Pics/截屏2023-02-14 下午2.41.56.png" alt="截屏2023-02-14 下午2.41.56" style="zoom:50%;" />

## Teams

麦克风: 选择LoopBack Audio

* 线上参加会议人听到的声音

扬声器: 选择 Macbook扬声器(或声卡)

* Teams线上其他人说话的声音
* 如果仅用做对讲, 使用电脑扬声器即可(或者摄像头的对讲扬声器)
* 如果需要音箱扩出来则选择声卡

<img src="./OnlineTrainin_TeamsSoundCardSettings_Pics/截屏2023-02-14 下午2.33.30.png" alt="截屏2023-02-14 下午2.33.30" style="zoom: 50%;" />

## LoopBack

在Device中

* Sources: 
  
  1. 添加声卡的Input1、2, 然后给连接到Output Channel
     * Mic信号
  
  2. Pass-Thru 连接到Output Channel
     * MacBook音频信号
  
* Output Channels: 混合信号作为Teams输入

* Monitors: 选择声卡的Output

  * 监听本地声音


<img src="./OnlineTrainin_TeamsSoundCardSettings_Pics/截屏2023-02-14 下午2.33.08.png" alt="截屏2023-02-14 下午2.33.08" style="zoom:50%;" />

---

其他: 

* 使用loopback功能后延迟会变大
* 声音经过网络压缩后其他人听到的音质未知
