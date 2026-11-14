# 声线与翻唱模型

## 豆包情绪版对白参考

2026-10-18 版本，每人八种情绪。样本为豆包声音复刻 2.0 合成音频，按角色和情绪命名，供试听参考。

| 情绪 | 麦麦 | 糖糖 |
| --- | --- | --- |
| 自然 | [试听](../assets/voice/maimai_natural.wav) | [试听](../assets/voice/tangtang_natural.wav) |
| 高兴 | [试听](../assets/voice/maimai_happy.wav) | [试听](../assets/voice/tangtang_happy.wav) |
| 生气 | [试听](../assets/voice/maimai_angry.wav) | [试听](../assets/voice/tangtang_angry.wav) |
| 疑惑 | [试听](../assets/voice/maimai_confused.wav) | [试听](../assets/voice/tangtang_confused.wav) |
| 委屈 | [试听](../assets/voice/maimai_hurt.wav) | [试听](../assets/voice/tangtang_hurt.wav) |
| 害羞 | [试听](../assets/voice/maimai_shy.wav) | [试听](../assets/voice/tangtang_shy.wav) |
| 惊讶 | [试听](../assets/voice/maimai_surprised.wav) | [试听](../assets/voice/tangtang_surprised.wav) |
| 调侃 | [试听](../assets/voice/maimai_teasing.wav) | [试听](../assets/voice/tangtang_teasing.wav) |

## RVC 翻唱

仓库选定 2026-10-29 的长素材 RVC v2「歌唱加强版」作为麦麦和糖糖的翻唱模型。每个角色包含权重和检索索引。糖糖版的制作记录显示，先用说话与歌唱混合素材训练，再做歌唱加强。

麦麦《カタオモイ》全曲和声 v4 及其局部精修使用的是 SoulX-Singer（`model-svc.pt`），以《活动小丑》50–70 秒的麦麦人声作参考。该工作流与下表的独立 RVC 声库分开记录。

| 角色 | 权重 | 检索索引 |
| --- | --- | --- |
| 麦麦 | [PTH](../assets/voice/rvc/maimai_extended_singing_v2.pth) | [索引](../assets/voice/rvc/maimai_extended_singing_v2.index) |
| 糖糖 | [PTH](../assets/voice/rvc/tangtang_extended_singing_v2.pth) | [索引](../assets/voice/rvc/tangtang_extended_singing_v2.index) |

用兼容的 RVC 工具选择同角色的两个文件，并使用有权处理的干声输入。麦麦版已用本仓库所附权重和索引完成《カタオモイ》全曲对照并经作者选定。糖糖版此前完成过《心跳不止》片段换声试听。公开文件供了解项目和试听。二次分发、训练和商用请先联系作者确认具体使用范围。
