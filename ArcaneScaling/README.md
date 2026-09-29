# ArcaneScaling

## 背景与目标
通过装备上的自定义附魔增强法术效果，使附魔强度能够映射为法术 Magnitude 和符合条件的 Duration 加成。

关键原则：在效果生成/应用阶段调整本次效果，不在目标掉血后补伤害。预期尽量融入原生处理流程，但具体 Hook 时序和兼容性必须通过实验确认。

## 计划产物
- ArcaneScaling.esl：自定义附魔、魔法效果、关键词、测试装备和配方。
- SKSE/Plugins/ArcaneScaling.dll：识别施法者装备上的自定义附魔，缩放符合条件的效果实例。
- 可选 SKSE/Plugins/ 下配置：系数、学派/效果范围；INI 或 JSON 待决定。

以上均为计划，当前没有可安装插件、DLL 或有效构建命令。

## 初版非目标
不做追加伤害补偿、全局基础法术重写、任意第三方法术的自动兼容承诺；不默认支持所有平台/运行时、VR、NPC、卷轴、法杖或全部效果类型。

## 文档
- [实现约束](AGENTS.md)
- [环境与依赖](ENVIRONMENT.md)
- [进度与交接](STATUS.md)
- [设计与阶段规划](docs/DESIGN.md)
- [决策记录](docs/DECISIONS.md)
- [测试与证据](docs/TESTING.md)
