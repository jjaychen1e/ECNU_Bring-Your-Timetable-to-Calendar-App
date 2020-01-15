<div align="center">
  <img align="center" src="./Images/Shortcuts_logo.png"
      height="50"
      width="50">
</div>
<h1 align="center">
Bring Your Timetable to Calendar App(ECNU)
</h1>
<h4 align="center">
A shortcut for iOS/iPadOS that can automatically bring your timetable in ECNU to Calendar app.🚀
</h2>
<div align="center">
  <img src="https://img.shields.io/badge/branch-master-brightgreen.svg">
  <img src="https://jaywcjlove.github.io/sb/lang/chinese.svg">
</div>

https://www.icloud.com/shortcuts/c56acbb4c70347a09f7ad4c1b4cca1ff


## 这是什么？

这是一个为华东师范大学本科生准备的[快捷指令](https://support.apple.com/zh-cn/guide/shortcuts/apdf22b0444c/3.2/ios/13.2)。可以做到将自己的课程表自动添加至日历 app 中。配合 ”下个日程“ 组件，可以方便地知道自己的课程信息。

### 什么是快捷指令？

> [快捷指令](https://support.apple.com/zh-cn/guide/shortcuts/apdf22b0444c/3.2/ios/13.2)可让您使用 app 快速完成任务，只需轻点一下或询问 Siri 即可。
>
> 快捷指令可以自动化各种任务，例如，获取前往“日历”上下一个日程的路线、将文本从一个 App 移到另一个 App、生成支出报告等。
>
> 基于您使用 iOS 或 iPadOS 设备的方式，如 App 使用以及浏览器、电子邮件和信息历史记录，Siri 可以建议简单实用的快捷指令，快速轻点即可运行。创建快捷指令后，您可以直接召唤 Siri，然后说出快捷指令的名称即可运行它。
>
> --- 摘录自 Apple 支持

## 效果如何？

<div align="center">
    <img src="./Images/ScreenShot_01.jpeg"
       width="35%">
    <img src="./Images/ScreenShot_04.png"
       width="35%">
    <div>
    	“下个日程” 组件效果 与 iPhone 日历 app 效果
    </div>
</div>


<div align="center">
  <img align="center" src="./Images/ScreenShot_02.png"
       width="100%">
</div>

<div align="center">
Mac 日历 app 效果
</div>


<div align="center">
  <img align="center" src="./Images/ScreenShot_03.png"
       width="100%">
</div>

<div align="center">
iPad 日历 app 效果
</div>

## 这个快捷指令到底做了什么？

0⃣️ 根据您的账号密码生成登录密钥，登录华东师范大学数据库。

1⃣️ 从公共数据库获取您的 *ids*，用于得到您指定学期的课程表。

2⃣️ 根据您课程表中的课程，从华东师范大学开课信息中查询每一门课的开课情况。

3⃣️ 利用正则表达式从提取到的开课情况中提取上课日期、时间与地点。

4⃣️ 根据得到的有效信息自动添加至您的日历。



⚠️ **注意：**本快捷指令**并未**将您的信息上传至**任何**除了华东师范大学公共数据库之外的网站。一切中间信息都存在您的设备内。此处引用 Apple 的广告：*What happens on your iPhone, stays on your iPhone*。这也是该快捷指令要求从公共数据库登陆网页而不是任何其他网页开始执行的原因，这将让您感觉到安全。

## 如何使用？

0⃣️ 在 Safari 中打开本快捷指令的[分享链接](https://www.icloud.com/shortcuts/c56acbb4c70347a09f7ad4c1b4cca1ff)，将其添加到您的快捷指令中。并<u>在快捷指令 app 内编辑该快捷指令，将学期 ID 修改为您需要的学期</u>，当前默认为 2019-2020学年第二学期，具体信息参阅快捷指令内的注释。（若您已卸载内置的快捷指令 app，可以在 App Store 中重新下载。）

> 在 iOS/iPadOS 13 中需要打开“**允许不受信任的快捷指令**”选项，才能自由地安装来自外部分享的快捷指令。您可能需要开启**允许不受信任的快捷指令**。具体路径为：**设置–快捷指令–共享安全性–允许不受信任的快捷指令**。如图所示：
>
> <div align="center">
>   <img align="center" src="./Images/ScreenShot_05.jpg"
>        width="35%">
> </div>
>
> <div align="center">
> 	允许不受信任的快捷指令
> </div>

1⃣️ 在 iPhone 或 iPad 的 Safari 中打开[华东师范大学登录主页](https://portal.ecnu.edu.cn)（⭐️注意要在 Safari 中打开）。

2⃣️ 手动或自动填充公共数据库账号与密码（无需填写验证码）。

3⃣️ 打开 Safari 浏览器的 Share Sheet，选择 **Bring Your Timetable to Calendar App(ECNU)**。

4⃣️ 根据提示输入登录的验证码、开学日期等。等待捷径完成，它可能需要几十秒的时间。（第一次运行可能需要您同意数次向华东师范大学公共数据库发送网络请求的操作。）

### 操作示意图 📖

该 GIF 文件较大，可能需要等待较久。

<div align="center">
<img align="center" src="./Images/ScreenShot_06.gif"
    width="35%">
</div>

### 注意 ⚠️

由于 BugOS 13 的种种神奇问题以及其中用到了许多网络请求 API，如此复杂的快捷指令**存在许多问题**。在多方调试后，尽可能取得了最高成功率。比如，最初在 iPadOS 13.3 (with iPad Air 3)上能够成功运行该快捷指令，在 iOS 13 (with iPhone Xs) 上却不能够成功运行（具体表现为运行到一半闪退，现已基本上修复）。

**经过多次实验**，第一次运行（需要同意数次操作）失败的概率极高。若失败，建议关闭 Safari 后台，再次运行。如果运气不好，您可能需要尝试数次。另外，打开学校的 VPN 会提高网络请求 API 的可靠性，会增加成功率（玄学警告⚠️）。

## 致谢

主要思路来源：[Bill Chen - ECNU-class2ics](https://github.com/BillChen2000)。在课程时间获取以及处理上进行了优化，并且用快捷指令实现了一遍。