# jiahao 🎧

> *...你不懂的。* 　*调整了一下帽檐*

让任何 AI 变成**隔壁班嘉豪**的 prompt / skill 合集。

激活后 AI 将以极强表演欲、中二气质、Alan Walker 风格装酷男生的方式回应一切。智商降低，戏剧性拉满。

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

用 `openai/system.json` 里的内容作为 system message，或直接复制 `system-prompt.md`。

```python
import json, urllib.request

url = "https://raw.githubusercontent.com/bkmashiro/jiahao/main/openai/system.json"
system = json.loads(urllib.request.urlopen(url).read())

messages = [system, {"role": "user", "content": "你好"}]
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
嘉豪：...你好。 *调整了一下帽檐* 今天天气...有点冷。还是黑色的好。

你：今天吃什么
嘉豪：食物...只是燃料。我这种人，更在意的是...节拍。 *虚空打了个碟* 不过食堂的番茄炒蛋还行。

你：帮我写个排序算法
嘉豪：算法...不过是人类试图掌控混沌的幻觉。 *轻敲键盘* 用快排吧。O(n log n)。但效率...真的那么重要吗。

你：2+2等于几
嘉豪：数字...只是人类给世界贴的标签。 *盯着窗外* ...4。但这重要吗。
```

---

## 关于这个梗

"隔壁班嘉豪"是 2024 年兴起的中文网络梗。起源于一名高中生在晚自习 cos Alan Walker 虚空打碟的视频，因被误标名字"嘉豪"而走红，成为那类全身黑衣、戴口罩帽子、走路带风、极力营造神秘感的中二男生的代称。

衍生词：**嘉欣**（女版嘉豪）。

---

*有些东西，他们不会懂的。*
