# 微信语音输入隐藏复制框 IME 隔离更新 1.0.11

2026-10-24 · Althy；保留原作者 DRHW。

每次 WriteClipboard 前执行 ImmAssociateContextEx(copySource.Handle, 0, 0)，仅解绑隐藏 scratch 的 IME 上下文。不使用 ImeMode.Disable，不关闭或销毁 receiver context；不改变全局快捷键、接收框、状态机、原生 Copy 和复制时机。保留既有 MaxLength、sequence/Unicode 校验、迟到提交、失败缓存及重试。

用户反馈另一台电脑 Ctrl+Alt+` 无法切换语音开始／结束，原因尚未确定。隔离测试证实原 scratch 共享 IMC，新方案解除该关联；实际快捷键尚未测试，不能宣称该故障已根治。真实向日葵端到端效果以用户复测为准。绿色倒置图标、清单功能字段、启动与停止替换流程保持；最低客户端 0.32.20，当前客户端 0.32.22 不变。

- 源码提交：`66fa4d45e7bb2fba0571f57d3ea104e3f033f59b`
- 新包：`packages/wetype-awesun-bridge/1.0.11.zip`
- ZIP SHA-256：`5e19daa8f8867a517b18419005f5daf9be9e55f314aa572dfec26dc874f5bf9d`
- 程序 SHA-256：`e06d68b169a89c4157fe315fedb188a89bdcf4dbd15be49da240015a7640a05e`

旧 ZIP 保留，其他插件条目不变；各渠道分别继承旧日志。此文件描述载荷，实际发布与安装状态见独立回执。
