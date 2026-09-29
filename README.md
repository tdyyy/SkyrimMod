# Skyrim Mod 工作区

目标游戏：上古卷轴 V：天际 特别版。每个业务子目录是一个独立 Mod；根目录仅保存协作规则与仓库配置。

| Mod | 用途 | 阶段 |
| --- | --- | --- |
| [ArcaneScaling](ArcaneScaling/README.md) | 装备附魔驱动的法术强度与持续时间增强 | 规划；未实现 |

## 新环境接手
1. 阅读 [AGENTS.md](AGENTS.md) 与目标 Mod 的说明、环境、进度文件。
2. 对照 ENVIRONMENT.md 核对环境；TBD 不可当作默认版本。
3. 配置本机路径，按记录恢复工具与依赖；不直接部署到真实游戏。
4. 从 STATUS.md 的下一步开始，执行可用验证，结束前更新交接。

## 新建 Mod
建立独立目录，并按 AGENTS.md 的必需文件清单补齐背景、环境、进度、设计、决策、测试文档。可参考 ArcaneScaling 的组织方式，但不得照搬其游戏机制或兼容性结论。

## 文件约定
- 文档使用中文，标识符/代码按项目约定；文本 UTF-8。
- Mod 内建议使用 src/、include/、tests/、scripts/、content/、config/、docs/；有实际内容时再创建。
- build/、out/、dist/ 为可再生产物，不入库。
- content/ 保存有意维护的插件内容源；不要全局忽略 .esl/.esp，以免遗漏权威源文件。
- 大型二进制/资产引入前确认许可与版本管理方案。
