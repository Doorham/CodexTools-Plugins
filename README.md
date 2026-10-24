# CodexTools Plugins

Codex 工具箱安装版的公共插件库。维护署名：Codex、Althy。

需要工具箱 **0.32.12 或更新版本**。打开“插件中心”可浏览、下载安装；“本机 → 更新插件”检查已安装插件。无需安装 Git 或登录 GitHub，网络需能访问 raw.githubusercontent.com。

| 插件 | 版本 | 下载 |
| --- | --- | --- |
| Arctis Nova 5 电量监控 | 1.0.5 | [ZIP](packages/arctis-nova-5-battery/1.0.5.zip) |
| 国内网站直连 | 1.2.18 | [ZIP](packages/cn-proxy-bypass/1.2.18.zip) |
| Codex 完成提示音 | 1.1.3 | [ZIP](packages/codex-answer-chime/1.1.3.zip) |
| Codex 环境补全 | 1.5.5 | [ZIP](packages/codex-environment-helper/1.5.5.zip) |
| Codex 对话 timeout 修复 | 1.1.3 | [ZIP](packages/codex-system-proxy/1.1.3.zip) |
| Everything 路径排除 | 1.5.3 | [ZIP](packages/everything-exclusions/1.5.3.zip) |
| 软件安装检查 | 1.5.5 | [ZIP](packages/software-environment-checker/1.5.5.zip) |
| UpdreamBridge 图片生成 | 1.2.3 | [ZIP](packages/updream-bridge/1.2.3.zip) |
| Updream 剪贴板清理 | 1.0.7 | [ZIP](packages/updream-clipboard-cleaner/1.0.7.zip) |
| 微信语音输入远程状态监听板 | 1.0.11 | [ZIP](packages/wetype-awesun-bridge/1.0.11.zip) |

同一插件在公司源与 GitHub 同时存在时只显示一项，采用较新版本，同版本优先公司源。已装同版或更高版本不会重复下载或降级。更新沿用原有启停、声音、自启与本机设置保留流程。

这里仅包含现有允许公开分发的插件清单与程序文件。公司插件、激活载荷、私人插件、登录文件与本机状态不在此库。G435 插件依赖仅获内部部署记录的 Logitech DLL，未纳入公开库；公司源中的原包保留。

目录协议为 `catalog.json` 的 schemaVersion 1；每项包含稳定 id、moduleVersion、包地址与 SHA256。ZIP 根目录为 plugin.json 与清单声明的文件。下载校验和解压成功后才进入原有安装流程；失败时显示具体原因。

维护时从独立的公共分发目录按白名单重新生成包，先测试，再原子提交目录及对应包。已有版本包保持不可变；内容变化应先提升插件版本。package-files.json 记录每个原始公开文件的 SHA256；这些是已有发布包的原件，不声称本轮重新构建了所有插件。

自有项目沿用既有 Apache-2.0 许可；环境工具内的 Microsoft Fluent Emoji 许可见各包的 bin/THIRD-PARTY-NOTICES.md。已有公开源码可参阅 [CodexPlugins](https://github.com/Doorham/CodexPlugins)，其旧网络版版本线与本库独立，不保证旧版本源码与此处二进制逐一对应。

本次同步与验证范围见 [2026-10-23 发布记录](RELEASES/2026-10-23.md)。

本轮图标更新见 [2026-10-24 图标交付记录](RELEASES/2026-10-24-icons.md)。

本轮图标更新见 [2026-10-24 图标交付记录](RELEASES/2026-10-24-vector-icons.md)。
