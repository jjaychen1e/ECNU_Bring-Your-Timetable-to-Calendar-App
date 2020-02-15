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

![封面](https://cdn.jsdelivr.net/gh/JJAYCHENFIGURE/Image/img/A01/2020-02-12-20-12-23.jpeg)

捷径社区：
[https://sharecuts.cn/shortcut/4812](https://sharecuts.cn/shortcut/4812)

快捷指令 iCloud 共享链接:
 [https://www.icloud.com/shortcuts/ed50ac2d016c47a58b5407fc383b166e](https://www.icloud.com/shortcuts/ed50ac2d016c47a58b5407fc383b166e)

（⚠️注：捷径社区是第三方快捷指令托管平台。打开捷径社区后选择安装捷径即可；或者直接在 Safari 中打开 iCloud 共享链接）

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

0⃣️ 根据账号密码生成密钥，登录华东师范大学公共数据库。

1⃣️ 从公共数据库获取您的 *ids*，用于得到您指定学期的课程表。

2⃣️ 在课程表中获取您的课程列表，在开课信息中查询指定学期对应的开课信息。

3⃣️ 利用正则表达式从提取到的开课情况中提取上课日期、时间与地点。

4⃣️ 根据得到的有效信息自动添加至您的日历。



⚠️ **注意：**本快捷指令**并未**将您的信息上传至**任何**除了华东师范大学公共数据库之外的网站。一切中间信息都存在您的设备内。此处引用 Apple 的广告：*What happens on your iPhone, stays on your iPhone*。这也是该快捷指令要求从公共数据库登陆网页而不是任何其他网页开始执行的原因，这将让您感觉到安全。

## 如何使用？

[使用教程及注意事项](http://jjaychen.me/efficiency/bring-timetable-to-calendar)

## 致谢

主要思路来源：[Bill Chen - ECNU-class2ics](https://github.com/BillChen2000)。在课程时间获取以及处理上进行了优化，并且用快捷指令实现了一遍。