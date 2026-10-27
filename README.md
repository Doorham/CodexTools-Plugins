# CodexTools Plugins

Codex 工具箱安装版的公共插件库。维护署名：Codex、Althy。

需要工具箱 **0.32.12 或更新版本**。打开“插件中心”可浏览、下载安装；“本机 → 更新插件”检查已安装插件。无需安装 Git 或登录 GitHub，网络需能访问 raw.githubusercontent.com。

| 插件 | 版本 | 下载 |
| --- | --- | --- |
| Arctis Nova 5 电量监控 | 1.0.5 | [ZIP](packages/arctis-nova-5-battery/1.0.5.zip) |
| 国内网站直连 | 1.2.19 | [ZIP](packages/cn-proxy-bypass/1.2.19.zip) |
| Codex 完成提示音 | 1.2.0 | [ZIP](packages/codex-answer-chime/1.2.0.zip) |
| Codex 环境补全 | 1.5.9 | [ZIP](packages/codex-environment-helper/1.5.9.zip) |
| Codex 对话 timeout 修复 | 1.1.3 | [ZIP](packages/codex-system-proxy/1.1.3.zip) |
| Everything 路径排除 | 1.7.5 | [ZIP](packages/everything-exclusions/1.7.5.zip) |
| 软件安装检查 | 1.5.9 | [ZIP](packages/software-environment-checker/1.5.9.zip) |
| UpdreamBridge 图片生成 | 1.2.4 | [ZIP](packages/updream-bridge/1.2.4.zip) |
| Updream 剪贴板清理 | 1.0.7 | [ZIP](packages/updream-clipboard-cleaner/1.0.7.zip) |
| 微信语音输入远程状态监听板 | 1.0.15 | [ZIP](packages/wetype-awesun-bridge/1.0.15.zip) |

同一插件在公司源与 GitHub 同时存在时只显示一项，采用较新版本，同版本优先公司源。已装同版或更高版本不会重复下载或降级。更新沿用原有启停、声音、自启与本机设置保留流程。

这里仅包含现有允许公开分发的插件清单与程序文件。公司插件、激活载荷、私人插件、登录文件与本机状态不在此库。G435 插件依赖仅获内部部署记录的 Logitech DLL，未纳入公开库；公司源中的原包保留。

目录协议为 `catalog.json` 的 schemaVersion 1；每项包含稳定 id、moduleVersion、包地址与 SHA256。ZIP 根目录为 plugin.json 与清单声明的文件。下载校验和解压成功后才进入原有安装流程；失败时显示具体原因。

维护时从独立的公共分发目录按白名单重新生成包，先测试，再原子提交目录及对应包。已有版本包保持不可变；内容变化应先提升插件版本。package-files.json 记录每个原始公开文件的 SHA256；这些是已有发布包的原件，不声称本轮重新构建了所有插件。

自有项目沿用既有 Apache-2.0 许可；环境工具内的 Microsoft Fluent Emoji 许可见各包的 bin/THIRD-PARTY-NOTICES.md。已有公开源码可参阅 [CodexPlugins](https://github.com/Doorham/CodexPlugins)，其旧网络版版本线与本库独立，不保证旧版本源码与此处二进制逐一对应。

本次同步与验证范围见 [2026-10-23 发布记录](RELEASES/2026-10-23.md)。

本轮图标更新见 [2026-10-24 图标交付记录](RELEASES/2026-10-24-icons.md)。

本轮图标更新见 [2026-10-24 图标交付记录](RELEASES/2026-10-24-vector-icons.md)。

## Everything 1.7.0 · 2026-10-26 · Doorham

路径卡片新增“吞噬上级”，确认后提升排除范围并合并被覆盖卡片；包含“修复卡死”。此插件要求工具箱 0.32.24 或更新版本，推荐先安装公司 Software 下载区中的 0.32.25 Setup，再更新插件。[源码](sources/everything-exclusions/1.7.0.zip) · [发布记录](RELEASES/everything-exclusions/1.7.0.json)。

## Everything 1.7.1 · 2026-10-26 · Doorham

修复 Everything 不响应退出时只能报错的问题：经用户确认才结束原进程并恢复操作，取消保留规则和卡片；清理本次退出命令，结束前备份已保存配置。客户端 0.32.25 不变。143 项独立实例及界面检查通过。[发布记录](RELEASES/everything-exclusions/1.7.1.json)。

环境补全与软件安装检查1.5.6：按场景编码、Git初始化、独立检测与安全下载；见[更新记录](RELEASES/2026-10-26-environment-1.5.6.md)。已有客户端只更新插件，无需Setup。

环境补全1.5.7：UTF-8卡片新增“拨乱反正”，先备份后按系统区域修复全局强制UTF-8；保留手动入口，不改文档、不自动重启。软件安装检查同步共享程序版本。见[更新记录](RELEASES/2026-10-26-environment-1.5.7.md)。

环境插件1.5.8：修复配置未完成时顶部虚报齐全，两包新增Git首次配置说明；新机器必须本人首次填写提交身份并通过验证。编码和下载功能保留，客户端不升级。见[更新记录](RELEASES/2026-10-26-environment-1.5.8.md)。

插件界面更新：Everything 1.7.3、环境两项 1.5.9、UpdreamBridge 1.2.4；保留原功能和本机设置，见[交付记录](RELEASES/2026-10-26-modern-ui.md)。Everything [对应源码](sources/everything-exclusions/1.7.3.zip)。

Everything 1.7.4：共享配置附带 JPG 缩略图，接收端独立缓存，保留本机封面及旧路径兼容。原上传端使用原署名重新上传一次，再由接收端同步。独立更新插件，无需升级客户端。见[发布记录](RELEASES/2026-10-26-everything-1.7.4.md)与[对应源码](sources/everything-exclusions/1.7.4.zip)。

Everything 1.7.5：连续清除共用一次规则事务，等待退出时追加的清除一并处理，保持FIFO边界与整批失败恢复；JPG共享保持。独立更新插件，无需升级客户端。见[发布记录](RELEASES/2026-10-26-everything-1.7.5.md)与[对应源码](sources/everything-exclusions/1.7.5.zip)。
