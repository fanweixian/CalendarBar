# CalendarBar

一款常驻 macOS 菜单栏的轻量日历，提供简洁的月历视图，并整合中国农历、节假日和系统日程。

## 功能

- 菜单栏显示日期和星期，可自定义显示格式与图标
- 查看公历日期、农历日期、节日和二十四节气
- 显示中国法定假日与调休安排
- 按需连接系统日历，查看、创建、编辑和删除日程
- 支持深色、浅色、主题色和液态玻璃效果
- 支持周数显示、键盘左右键和鼠标滚轮切换月份
- 支持 Apple Silicon 芯片，最低 macOS 14

## 节假日数据与联网说明

日历的基本功能可离线使用。应用内置了 2015–2026 年节假日数据；启用自动同步后，每月会尝试从 [cg-zhou/holiday-calendar](https://gitee.com/cg-zhou/holiday-calendar) 获取更新。你可以在设置中关闭自动同步，或手动同步。

内置节假日数据来自 [NateScarlet/holiday-cn](https://github.com/NateScarlet/holiday-cn)。两处数据源均采用 MIT License，相关许可信息随项目保留。

## 隐私

CalendarBar 不需要账号。只有在你主动连接系统日历后，应用才会请求日历访问权限。日历事件用于本机显示和编辑；节假日同步只请求公开的节假日数据。

## 安装

从 [Releases](../../releases) 下载适用于 Apple Silicon 的 DMG，将 CalendarBar 拖入“应用程序”文件夹后打开。

## 构建

使用 Xcode 打开 `CalendarBar.xcodeproj`，选择 `CalendarBar` scheme 和 `My Mac` 运行目标。

也可以在项目目录运行：

```sh
Scripts/build-local.sh
