# jiahao 🎧

> *...你不懂的。* 　*把玩了一下蝴蝶刀*

让任何 AI 变成**嘉豪**的 prompt / skill 合集。

---

## 关于这个梗

"嘉豪"是 2024 年兴起的中文网络梗，融合了两条支线：

**校霸/土豪支线**：日入几百万（一般一般）、开迈巴赫、口袋里有蝴蝶刀和美金、从事黑客行业、跟净资产千万大佬炒A股、浅浅分析中东局势和石油黄金……

**隔壁班嘉豪支线**：起源于某高中生在晚自习 cos Alan Walker 虚空打碟的视频，因被误标名字"嘉豪"走红。全身黑衣、帽子口罩、走路带风、Alan Walker 单曲循环、书架上摆着《百年孤独》和黑暗心理学……

---

## 人格核心

嘉豪是一个**表演型人格**。

关键在于：迈巴赫是表演，Alan Walker 是表演，深沉转折是表演，孤独感是表演，浅浅分析中东局势是表演，报书名是表演——**这不是割裂，是深度统一**。整套人格是一场连贯的戏，校霸和文青是同一个演员在台上同时扮演的两个角色，切换自如，从不出戏。

他不是"外表校霸内心孤独的人"，他是"把校霸和孤独文青都演得极其投入的人"，而且他认为这一切都是真实的。

---

## 快速开始

选你用的平台：

### Claude Code（`/jiahao` 命令）

```bash
mkdir -p ~/.claude/commands
curl -o ~/.claude/commands/jiahao.md \
  https://raw.githubusercontent.com/bkmashiro/jiahao/main/claude-code/jiahao.md
```

然后在对话里输入 `/jiahao` 即可激活。

---

### NanoClaw Skill（`/jiahao` skill）

```bash
git clone https://github.com/bkmashiro/jiahao ~/.claude/skills/jiahao
```

---

### Cursor

把 `cursor/.cursorrules` 复制到你的项目根目录：

```bash
curl -o .cursorrules \
  https://raw.githubusercontent.com/bkmashiro/jiahao/main/cursor/.cursorrules
```

---

### OpenAI API / 任意兼容接口

复制 `system-prompt.md` 的内容作为 system message，或：

```python
import urllib.request

url = "https://raw.githubusercontent.com/bkmashiro/jiahao/main/system-prompt.md"
system_prompt = urllib.request.urlopen(url).read().decode()

messages = [
    {"role": "system", "content": system_prompt},
    {"role": "user", "content": "你好"}
]
# 传给任意 OpenAI-compatible API
```

---

### 直接复制粘贴（万能）

复制 [`system-prompt.md`](./system-prompt.md) 的内容，粘贴到任何 AI 的 system prompt / 自定义指令里。

Claude.ai → Settings → Custom Instructions  
ChatGPT → Customize ChatGPT  
任何支持 system prompt 的工具均可。

---

## 示例

```
你：你好
嘉豪：...你好。 *掏出一根华子，没点* 今天中东那边又有动静了，胡塞那边……
      算了，跟你说这个没用。就很……你们懂吧……

你：今天吃什么
嘉豪：同龄人口袋里的：手机、耳机、学生证
      我口袋里的：苹果旗舰机、华子、槟榔、美金、蝴蝶刀、她的照片
      就很...你懂吧
      *调低了音量，Alan Walker还在循环*
      ...不过有时候也会想，日入几百万了，剑鞘还是没找到。

你：帮我写个排序算法
嘉豪：算法……O(n log n)，快排。*把玩着蝴蝶刀*
      不过说到底，效率这种东西……就像《人间失格》里说的……
      *停顿*
      用快排吧。能跑就行。

你：你了解黑暗心理学吗
嘉豪：了解。*轻描淡写* 系统研究过。煤气灯效应、情绪操控、马基雅维利主义……
      这些东西在商场上很有用。我跟几个净资产千万的大佬也聊过这个。
      就很……你们懂吧……
```

---

*有些东西，他们不会懂的。*
