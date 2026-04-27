## 更新说明

<!-- Personal fork notes:
  - Using this for learning purposes / personal media downloading
  - Main interest: m3u8 parsing and the deep search feature
-->

### 2.6.6

[Updated] 感谢 @Oleada1 完善翻译

[Updated] 增强 深度搜索 现在可以找到更多资源

[Fixed] 修复 firefox无法视频录制问题

[Fixed] 修复 录制视频 无法弹出下载问题

[Fixed] 修复 深度搜索 导致网页无法正常使用问题

[Fixed] 修复 屏蔽列表 失效问题

[Fixed] 修复 edge Brave等浏览器 使用在线ffmpeg 文件为空问题

### 2.6.5

[Added] 部分网站不希望被本扩展抓取 添加 全局强制屏蔽 [屏蔽列表](https://o2bmm.gitbook.io/cat-catch/blockedsite)

[Added] 增加土耳其语 感谢 @ilker-binzet

[Added] 增加西班牙语 感谢 @Oleada1

[Fixed] 部分浏览器 侧边栏无法使用问题

[Fixed] 发送到 Aria2 User-Agent 传递错误

[Fixed] 模板标签替换 双引号处理错误

[Fixed] 导入配置时部分设置丢失问题

[Fixed] 深度搜索导致部分网站无法正常使用问题

### 2.6.4

[Updated] webrtc 录制脚本 更新

[Updated] 深度搜索脚本 更新

[Updated] 更新日语 感谢@hmaoraze

[Added] 支持 MQTT 协议 感谢@jetsung

[Added] 筛选 删除重复文件名

[Added] 始终打开 深度搜索 选项 (慎用)

[Added] 弹出模式 可选择页面

[Added] 筛选页面 支持时长排序

### 2.6.3

[Fixed] Chromium 114 版本以下缺少 `sidePanel` 功能，导致扩展无法使用

### 2.6.2

[Added] m3u8 解析器 录制失败重试功能 (测试)

[Added] m3u8 解析器 尝试估算文件大小

[Added] 增加 其他设置 `使用侧边栏` 选项。从 popup 模式改为浏览器侧边栏打开扩展 (不支持 firefox)

[Updated] m3u8 预览现在支持 hevc/h265 编码

[Updated] 深度搜索 支持解析 vimeo playlist.json

[Changed] 重构 缓存捕捉 脚本 减少头部数据缺失问题

[Changed] 重构 排除重复的资源 减少资源占用

[Fixed] 缓存捕捉脚本导致视频无法播放问题

[Deleted] m3u8 解析器 删除了旧版本下载器

[Deleted] 启用新弹出页 删除旧弹出页

### 2.6.1

[Changed] 对手机浏览器进行一些适配

### 2.6.0

[Added] 全新的弹出页面(`弹出`按钮) 文件预览/筛选帮助你下载需要的文件 (设置`feat newPopup`关闭新版)

[Changed] 增强数据发送功能，现在能自定义发送数据 感谢 @helson-lin 的支持

[Changed] 正则匹配 现在能获取到请求头

[Changed] 支持夸克浏览器 (部分功能不可用)

[Updated] 深度搜索脚本 找到更多资源

[Fixed] Fifefox 导入功能 bug 导致扩展不可用

[Fixed] 偶尔会弹出多个 ffmpeg 页面的 bug

[Fixed] 下载器 打开`边下边存` 无法自动关闭的 bug

### 2.5.9

[Added] 增加屏蔽网址功能 添加不希望开启扩展的网站 (可设为白名单, 只允许添加网址开启扩展)

[Fixed] 新版下载器 下载大文件时 出错 #610

[Changed] 限制每页面最大储存 9999 条资源

[Changed] 设置增加导航栏

[Changed] 自动下载 允许自定义保存文件名

### 2.5.8

[Changed] 如果资源 url 不存在文件名 尝试使用页面标题作为文件名

### 2.5.7

[Fixed] 自定义保存文件名使用 `/` 无法创建目录

[Changed] firefox 升级 manifest v3

[Changed] firefox 128 以上版本 支持使用深度搜索 缓存录制 等脚本功能

[Fixed] firefox 无法发送到在线 ffmpeg 问题

[Added] 重构 猫抓下载器 如需旧版本请在设置 关闭 `Test version` 选项

[Added] `URL Protocol m3u8dl` `调用程序` 增加下载前确认参数设置

[Added] m3u8 为疑似密钥增加验证密钥功能

[Changed] 增强 深度搜索 现在能找到更多疑似密钥

### 2.5.6

[Fixed] m3u8 解析器 自动关闭 bug #531

[Fixed] chrome 130 自定义 url 新规范导致 `m3u8dl://` 调用失败 #528

[Fixed] m3u8 解析器 文件不正确无法解析 造成死循环占用 CPU 问题

[Changed] 猫抓下载器 添加更多请求头 增加下载成功率

### 2.5.5

[Fixed] 修复一个严重 bug #483

[Added] 在线 ffmpeg 提供服务器选择

[Fixed] m3u8 解析器 文件名存在`|`字符 无法下载问题

[Changed] 发送数据 提供完整请求头

### 2.5.4

[Added] m3u8DL 增加切换 RE 版本 (RE 版 需[URLProtocol](https://github.com/xifangczy/URLProtocol))

[Added] 录制相关脚本 增加码率设置

[Fixed] 深度搜索 脚本错误导致无法使用

[Fixed] m3u8 解析器录制直播 录制时间显示错误

### 2.5.3

[Added] 增加`弹出`模式 (以新窗口打开资源列表页面)

[Added] 增加`调用本地程序`设置, 程序没有调用协议, 可以使用[URLProtocol](https://github.com/xifangczy/URLProtocol)帮助程序注册调用协议。具体使用方法查看 [调用本地协议](https://o2bmm.gitbook.io/cat-catch/docs/invoke)

[Added] 下载器 增加`边下边存`选项 可以用来下载一些直播视频链接

[Added] 现在使用`深度搜索` 或其他脚本得到的疑似密钥, 直接显示在 popup 页面 `疑似密钥` 标签内。

[Added] 增加 葡萄牙语

[Changed] 重写 `录制webRTC` 脚本

[Changed] `m3u8解析器` `下载器`页面内更改设置不会被储存。所有设置更改统一到扩展设置页面。

[Changed] storage.local 更改为 storage.session 以减少 IO 错误导致扩展无法使用.(要求 chrome 104 
