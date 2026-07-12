<div align="center">

# 电车站.skill · Tramstop Skill

**人味不是删出来的。**
**De-slop your writing with evidence, not word blacklists.**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Agent Skills](https://img.shields.io/badge/Agent%20Skills-Standard-green)](https://agentskills.io)
[![Multi-Runtime](https://img.shields.io/badge/Runtime-Claude%20Code%20·%20Codex%20·%20Cursor%20·%20OpenClaw-blueviolet)](#安装)
[![Made with 女娲](https://img.shields.io/badge/Made%20with-弗洛伊德.skill-orange)](https://github.com/alchaincyf/freud-skill)

> AI编细节是为论点服务的，
> 不会把细节浪费在用不上的电车站上。

[为什么叫电车站](#为什么叫电车站) · [它凭什么不一样](#它凭什么不一样) · [两种用法](#两种用法) · [安装](#安装) · [English](#english)

</div>

---

## 为什么叫电车站

一次四版本盲测：同一篇文章的四个版本，匿名乱序，交给一位审过上千篇AI投稿、患有重度「AI疑心病」的编辑，让他赌哪版是真人手笔。

他赌中了。理由不是文笔，是一个对论证毫无用处的细节——作者在维也纳除了弗洛伊德博物馆，还去看了**阿德勒的电车站**。

那个电车站是作者两年前真实发过的动态。这个skill帮你的文字找回它的电车站。

## 它凭什么不一样

市面上的去AI味工具几乎都是「删」派：禁词表、句式黑名单、破折号计数。这个skill的方法论来自一次真实的对照实验（四版本改写×四评委盲测，数据在 [`references/evidence.md`](references/evidence.md)）：

| 方法 | 盲测得分（像真人，1-10） |
|------|------------------------|
| 原稿 | 5.5 |
| 纯删法（结构手术） | 5.9 —— 评委：「干净得像消过毒」 |
| **删法 + 真实素材注入** | **8.6，四票全胜** |

结论写在名字里：**人味不是删出来的**。AI味分四层（词汇 < 句式 < 结构 < 经验），删词只是及格线；真正的分界线在经验层——文字背后有没有站着一个具体的人。这与学术检测研究的结论一致：把词汇线索全部洗掉，熟练读者仍能100%识别AI文。

所以这个skill在「删」之外多做一件决定成败的事：**先问你要真实素材**（你的经历、你踩过的坑、你记得但说不上为什么记得的细节），再动笔。挖不到就放`[待补]`占位——它有一条铁律：**绝不编造你的经历**。

## 两种用法

| 模式 | 你说 | 它做 |
|------|------|------|
| **诊断** | 「这稿子AI味重吗？」 | 按四层扫描，输出分层报告：几个细节是可替换的？判断押注了吗？删掉修辞还剩多少信息量？ |
| **改写** | 「帮我改得像人写的」 | 挖素材（问你2-3个具体问题）→ 结构手术 → 经验注入 → 可选盲测验证 |

## 安装

```bash
# Claude Code（推荐放到全局 skills 目录）
git clone https://github.com/alchaincyf/tramstop-skill.git ~/.claude/skills/tramstop-skill
```

或者直接把仓库链接丢给你的agent，说一句「帮我安装这个skill」。

兼容 Claude Code / Codex / Cursor / OpenClaw 等支持 Agent Skills 标准的运行时。安装后说「去AI味」「这稿子读着不对劲」「太像AI了」即可触发。

## 背后的故事

作者的公众号被读者反馈「AI味越来越重」，试过禁词表、指定用语、模仿Paul Graham、投喂旧文，全部收效甚微。于是做了一次系统调研（学术文献+中英文实践圈+自家语料解剖）和一次四版本对照盲测，发现所有失效的方法都在打最浅的词汇层，而分界线在经验层。这个skill就是那次实验的可执行版本。完整故事见公众号文章（搜「花叔」）。

## 关于作者

**花叔 Huashu** — AI Native Coder，独立开发者，代表作：小猫补光灯（AppStore 付费榜 Top1）

| 平台 | 链接 |
|------|------|
| 🌐 官网 | [bookai.top](https://bookai.top) · [huasheng.ai](https://www.huasheng.ai) |
| 𝕏 Twitter | [@AlchainHust](https://x.com/AlchainHust) |
| 📺 B站 | [花叔v](https://space.bilibili.com/14097567) |
| ▶️ YouTube | [@Alchain](https://www.youtube.com/@Alchain) |
| 📕 小红书 | [花叔](https://www.xiaohongshu.com/user/profile/5abc6f17e8ac2b109179dfdf) |
| 💬 公众号 | 微信搜「花叔」或扫码关注 ↓ |

<img src="wechat-qrcode.jpg" alt="公众号二维码" width="360">

## 许可证

MIT — 随便用，随便改，随便造。

---

<div align="center">
<sub>作者的其他项目 · also by 花叔</sub>

[![FanBox · Coding Agent 的驾驶舱](https://raw.githubusercontent.com/alchaincyf/fanbox/master/assets/promo-banner.jpg)](https://github.com/alchaincyf/fanbox)

[女娲.skill — 蒸馏任何人的思维方式](https://github.com/alchaincyf/nuwa-skill) · [弗洛伊德.skill — 给AI做心理分析](https://github.com/alchaincyf/freud-skill) · [达尔文.skill — 让 Skill 无限进化](https://github.com/alchaincyf/darwin-skill)

</div>

---

## English

**Tramstop Skill** is an evidence-based de-slop skill for AI-assisted writing. Its method comes from a controlled experiment (4 rewrite strategies × 4 blind judges): word blacklists and structure surgery alone barely moved the needle (5.5 → 5.9 on a 10-point "reads human" scale), while injecting **traceable personal material** scored 8.6 with a unanimous vote.

The name: a judge with severe "AI suspicion" correctly identified the human-sounding version by one detail useless to the argument — the author had visited Adler's tram stop in Vienna. AI invents details that serve the point; humans remember details that serve nothing.

What it does differently:
- **Four-layer model**: vocabulary < syntax < structure < lived experience. Deleting AI-isms is table stakes; the deepest layer is the only one AI can't fake (consistent with Russell 2025: expert raters still catch humanized AI text at 100% via originality and structure).
- **Two modes**: diagnose (layered report) or rewrite (mine real material from you → structure surgery → experience injection).
- **Hard rule**: never fabricates your experiences — it asks, or leaves `[TODO]` placeholders.

Install: `git clone https://github.com/alchaincyf/tramstop-skill.git ~/.claude/skills/tramstop-skill` — works with Claude Code, Codex, Cursor, OpenClaw and other Agent-Skills-compatible runtimes.
