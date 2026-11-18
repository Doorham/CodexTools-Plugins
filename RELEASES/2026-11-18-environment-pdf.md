## 1.5.13 · LibreOffice 实际转 PDF 后判定就绪

软件安装检查在隔离配置目录用 LibreOffice 把一页文档导出为 PDF，并核对文件头、交叉引用及结束标记。程序、转换结果与 PATH 均通过才显示已就绪。LibreOffice 卡片的“转 PDF”可使用同一条路径处理本地文档。

本机故障发生在初始化崩溃报告时查询代理例外地址的 DNS 反向解析。仅导出进程使用 LibreOffice 的 CrashDumpEnable=false 启动选项，保留系统代理和用户日常 LibreOffice 配置。技术细节见 LibreOffice desktop/source/app/crashreport.cxx。两个环境插件独立更新至 1.5.13。

包含自 1.5.10 以来的下载源维护和卡片自助安装改进。安装方式：工具箱插件中心分别更新“Codex 环境补全”和“软件安装检查”。
