# Everything 1.7.5 · 2026-10-26 · Althy

连续清除卡片改为共用一次规则事务，保留原作者 Doorham。相邻清除请求合批；等待 Everything 正常退出期间追加的清除，会在开始读写配置前收进本批。批次冻结后新增的请求进入下一批，其他操作类型保持 FIFO 顺序边界，不跨越边界合并。

每项请求的去重、完成状态和队列上限保留。整批一次保存，失败时恢复原卡片顺序和实际移除规则；完整保存成功才清理缓存。队列与卡片仍在 UI 线程修改，没有通过人为延迟或更改退出超时实现合批。

保留 1.7.4 的 JPG 共享缩略图、旧 PNG 兼容、现代界面及默认 Everything 恢复策略；不改变客户端、图标或共享配置。包与 EXE 同为 1.7.5，最低客户端仍是 0.32.24，可独立更新插件。

232 项隔离完整业务回归及 17 项包生命周期校验通过，覆盖等待期间追加的独立 Everything 实例、冻结前后请求、FIFO 混排、重复/失效 ID、整批保存失败回滚、取消后停止队列及既有 JPG 功能。未清除真实用户目录、修改默认 Everything 实例或上传真实配置，不据此宣称其他员工设备已经更新。

源码包：[sources/everything-exclusions/1.7.5.zip](../sources/everything-exclusions/1.7.5.zip)，SHA256 50164732b61e2f7288a5f9d2e362841cc53dac5448c31aa4e23468ace996ddc6；基线为 1.7.4 源码归档。插件包 SHA256 3e4b4f2d2a272cf74adc4d19c9b3f2bf7b7530910a17e52b1981f2eecb0f4dfa，EXE SHA256 0063bcb773816327b3112f60018a6f9428efce90d2e7e520d3719ef9a18a6aa4。交接见包内 BATCH-REMOVAL.md、DEVLOG.md，逐文件摘要见 package-files.json；本机及渠道部署分别以回执登记。
