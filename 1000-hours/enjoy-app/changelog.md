# 版本更新

## v0.7.9

### 新增功能

- 内嵌社区

## v0.7.8

### 修复故障

- 修复部分样式问题
- 修复录音超过 40 秒发音评估结果缺失
- 修复导入文档时修改音色不生效

## v0.7.7

### 修复故障

- 修复 Unhandle Error 弹窗
- 分享录音失败
- 发音评估中原因发音播放异常

## v0.7.6

### 修复故障

- 修复弹窗被遮挡的问题

## v0.7.5

### 新增功能

- 文档阅读页面可以修改布局（水平或垂直）
- 文档可以打印当前页面（包含翻译）
- 跟读页面可以复制字幕全文（不含时间轴）
- 查单词面板新增单词的语音评估

### 修复故障

- 修复循环播放和重复播放时异常问题
- 修复复制粘贴等快捷键失灵的问题
- 修复语言评估结果部分按钮被遮挡无法点击的问题

### 其他

- 取消自动更新，改为手动检查更新

## v0.7.4

### 修复故障

- 修复部分 Windows 系统语音转文本导致卡死的问题

## v0.7.3

### 修复故障

- 增加更多必要日志，方便排查问题
- 修复导入音视频时，压缩选项不生效的问题

## v0.7.2

### 修复故障

- 修复发音评估弹窗布局问题

## v0.7.1

### 修复故障

- 修复布局问题

## v0.7.0

### 新增功能

- 增加导入文档功能，可跟读、翻译等，支持导入本地 epub, txt, markdown 等格式文本，同时支持在线文章导入
- 重构软件顶部栏和侧边栏
- 本地 whisper 增加更多配置项，可选择 `whisper.cpp` 版本
- 导入音视频时，增加是否压缩的选项
- 增加默认的 TTS 配置
- Mixin 可以选择扫码登录

### 修复故障

- 修复字幕旧格式导致的错误
- 重复导入相同资源时，将更新资源的修改时间，使其置于排序靠前
- 修复字幕中特殊符号（例如破折号）导致显示异常的问题

### 其他

- 重构部分代码，优化可维护性
- 优化 UI 样式

## v0.6.1

### 修复故障

- 修复部分用户导入音视频时报 `Foreign key constraint failed` 错误

## v0.6.0

### 新增功能

- 重构 AI 聊天，新增了指定回答、转发消息等多个功能
- 支持全局唤起聊天窗口，任何页面均可随时与 AI 对话
- 优化录音文件格式，体积大幅减少
- 支持一键删除录音文件，释放磁盘（保留录音时长记录）
- 支持将原智能助手对话迁移至聊天

### 修复故障

- 修复代理设置无法自动生效

### 其他

- 替换本地 whisper.cpp 组件为 onnxruntime 版本，增强兼容性
- 数据迁移以及每天启动时，自动备份数据库至本地

## v0.5.2

### 修复故障

- 创建语音文本时由于网络不佳导致创建失败

## v0.5.1

### 新增功能

- 支持导入 mdx 词典
- 跟读界面重构，可以拖动改变各区域大小
- 进入跟读时，自动查找并下载语音文本

### 修复故障

- Windows 下点击词典发音弹窗
- 更新代理时，网络状态不自动刷新

### 其他

- 优化了左侧栏布局，可以手动隐藏和展开

## v0.5.0

### 新增功能

- 支持导入第三方词典
- 支持将同一资源所有段落的录音合并下载
- 社区广场分享录音显示原始音频段落
- 支持越南语

### 修复故障

- 发音评估失败时，不弹出错误信息
- 修复重置按钮
- 修复聊天中请求失败时，不弹出错误信息

### 其他

- 重构配置文件，隔离多用户间的配置选项
- 优化软件打开流程，网络不佳时可以离线使用

## v0.4.1

### 新增功能

- 增加聊天中的 AI 建议
- 增加录音的高级配置项
- 可以打开配置文件
- 支持泰语

### 修复故障

- 修复朗读全文录音 1 分钟限制
- 社区广场中查单词弹窗错位
- 聊天窗口发送后清空文本框

### 其他

- 优化发音频评估结果中单词显示
- 优化部分错误提示
- 优化聊天的提示语

## v0.4.0

### 新增功能

- AI 语音聊天
- 下载 Youtube 视频时应用代理设置
- 网络状态检查
- 跟读播放速度支持快捷键
- 支持近期费用查询
- 本地资源库详情展示
- 一键清理源文件丢失的资源
- 发音评估页面支持分享录音
- 支持粤语

### 修复故障

- 修复因 AI 模型设置导致设置页面无法打开

### 其他

- 优化录音功能

## v0.3.4

### 修复故障

- 修复 OpenAI 设置模型无法使用
- 修复跟读页面播放器循环播放异常问题
- 修复网络不佳情况下 GPT 预设的加载
- 修复 Azure AI 语音转文本某些情况下卡死的问题
- 修复跟读页面播放器突然失灵的情况

## v0.3.3

### 新增功能

- 针对有背景音乐等噪声的音频，优化了字幕的对齐准确度
- 优化字幕修改，支持修改时间轴
- 视频播放器支持显示字幕
- OpenAI 设置支持自定义模型
- 充值支持加密货币链上支付

### 修复故障

- 自由录音进行发音评估报错
- Mixin 支付无法打开

### 其他

- 其他体验上的优化

## v0.3.2

### 新增功能

- 可以修改 API 网址

### 修复故障

- 字幕首个单词闪动

## v0.3.1

### 新增功能

- 社区广场分享录音显示评估分数
- 课程显示章节完成人数
- 音视频字幕可导出为 PDF（带音标）
- 社区广场可以点赞
- 语音转文本可以从云端下载已有的字幕

### 修复故障

- 录音对比不起作用
- 课程发音评估结果不显示
- 侧边栏在小窗口的显示

### 其他

- 优化了发音评估流程

## v0.3.0

### 新增功能

- 互动式课程

### 修复故障

- 语音转文本时出现网络错误后卡死
- 发音评估部分音标显示不正常

## v0.2.14

### 新增功能

- 智能助手对话中可以选择 TTS 语言
- 语音转文本提取人声（实验性功能）

### 修复故障

- 发音评估在深色主题中的样式问题
- 语音转文本时有原始文本时不再重新识别

### 其他

- 优化语音转文本的设置，隐藏高级选项
- 优化添加本地资源处理的结果与报错

## v0.2.13

### 新增功能

- 语音转文本时可以自定义设置，包括上传字幕文件
- 发音评估列表增加排序
- 音频/视频列表页增加排序、筛选和搜索

## v0.2.12

### 修复故障

- Windows 版本数据库更新异常

## v0.2.11

### 新增功能

- 增加发音评估的独立页面，支持无文本录音评估，及上传录音文件评估
- 增加发音评估快捷键，默认为 `A`
- 快捷键设置最多支持三个键（如 `Ctrl`+`Shift`+`A`）
- 跟读页面自动记录上次跟读句子

### 修复故障

- OpenAI TTS 使用 `tts-1-hd` 时报错
- 快捷键失灵
- 网络环境不佳时，手机验证码无法点发送
- 广场页面，多个录音同时播放
- 使用本地 whisper 进行语音转文本时，无法中断进程
- 音标字体加载失败

### 其他

- 优化跟读页面 UI

## v0.2.10

### 新增功能

- 支持 Azure TTS，支持多语言、多角色

### 修复故障

- 除英语以外，其他语言的音标不做修正
- 下载音频时指定后缀
- 修复下拉菜单过长时无法拖动的问题
- 调整录音修剪阈值，避免录音过度剪切

### 其他

- 新用户默认以 azure 作为 STT 引擎

## v0.2.9

### 新增功能

- Mixin 充值支持多种加密货币
- 支持设置多种“学习语言”

### 修复故障

- 修复“朗读全文”时的录音计时问题
- 修复 echogarden 报错 "No match found in uncrop timeline"

## v0.2.8

### 修复故障

- 智能助手对话进入跟读页面时，点击任意按钮自动退出

## v0.2.7

### 新增功能

- 朗读全文模式
- 新增 Youtube 频道作为视频资源

### 修复故障

- 智能词典无法查询
- 时间的显示及统计不遵循本地时区
- audible.com 的音频资源加载失败
- 网速不佳时新建智能对话失败

### 其他

- 升级 whisper.cpp 版本至 [v1.6.0](https://github.com/ggerganov/whisper.cpp/releases/tag/v1.6.0)

## v0.2.6

### 新增功能

- 更新模型列表，支持 GPT-4o 模型
- EnjoyAI 增加除 OpenAI 以外的其他模型(例如 gemini-pro-1.5 等)
- 支持颗粒度更小的 AI 模型设置，可以对“智能词典”单独设置模型

### 修复故障

- Mixin 登录页面深色模式下的样式
- 音标重音标注符号修改至辅音

### 其他

- 优化了智能助手列表
- 支持通过 API 更新模型列表

## v0.2.5

### 修复故障

- Mixin ID 为 5 位数时无法发送验证码

## v0.2.4

### 新增功能

- 本地 whisper 模型支持识别英语以外的语言（需要选择不带 `.en` 的模型）
- 跟读页面做笔记功能
- 修改语音文本功能
- 对语音进行 AI 提炼标题
- 全局查词典和智能翻译（选中文本后右键菜单选择）
- 生词本支持快捷键
- 下载任意选段音频

### 修复故障

- 暗黑模式下部分样式问题
- 原文以 `-` 开头时语音转文本报错
- 跟读页面快捷键失灵
- 代理设置无法保存
- 录音超时后没有自动停止
- 导入资源时后缀大写时报错
- Youtube 视频无法下载
- 录音不完整问题

### 其他

- Github 登录改为设备验证流程
- Mixin 登录改为验证码方式
