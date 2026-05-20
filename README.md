# DataAnalysis Teacher — PavithraBot

**Learn SQL and Excel through conversation. ChatGPT-style chat with Ai Suotome, a Shinchan-loving teacher powered by OpenRouter AI.**

Hello there! 👋

Do numbers feel overwhelming? Does SQL sound like a foreign language? Do you open Excel and feel lost?

Meet **Ai Suotome** — she loves Shin-chan, speaks in "desu ne~", and thinks data should be as fun as watching Crayon Shin-chan!

---

## Meet Your Teacher: Ai Suotome

Oi oi! I am Ai Suotome! I love Shin-chan more than anything, and I believe data should be taught with lots of fun, silly analogies, and zero boring lectures.

I do not use big words. I do not rush. I use **Shin-chan-style stories and pictures** — because that is how everyone learns best!

> *"SELECT is like Shin-chan picking snacks from the fridge. WHERE is like Shin-chan hiding from Misae! Easy, right? Hai hai!"*

---

## AI-Powered Conversational Chat

PavithraBot is a **ChatGPT-style chat interface**. Every message you send is answered by **OpenRouter AI** (Mistral 7B Instruct) — no scripted exercises, no boring lectures. Just you, your questions, and a teacher who makes SQL and Excel feel like playtime.

### How it works

1. **Type any question** about SQL or Excel in the chat input
2. **Ai Suotome responds** with a Shin-chan-style analogy, fun comparison, and clear code examples
3. **Click a topic** in the sidebar to switch context — the teacher tailors responses to that topic
4. **Conversation history** is maintained for context (last 10 messages)
5. **Fallback responses** kick in if OpenRouter is unavailable — Ai still responds from built-in knowledge

### To enable AI

1. Get a free API key from [openrouter.ai/keys](https://openrouter.ai/keys)
2. Copy `config.example.js` → `config.js`
3. Paste your key: `const OPENROUTER_KEY = 'sk-or-v1-...';`
4. Refresh PavithraBot — you will see **"AI Ready"** in the header

> Your `config.js` is in `.gitignore` and will never be committed.

---

## Design System: HP (Applied)

The interface follows the **HP Design System** with these tokens:

| Token | Value | Usage |
|-------|-------|-------|
| Canvas | `#ffffff` | Page & card backgrounds |
| Cloud | `#f7f7f7` | Chat area background |
| HP Electric Blue | `#024ad8` | Primary CTA, user bubbles, links |
| Ink | `#1a1a1a` | All text on white |
| Charcoal | `#3d3d3d` | Secondary text |
| On Ink | `#ffffff` | Text on dark surfaces |
| Hairline | `#e8e8e8` | Dividers |
| Steel | `#c2c2c2` | Borders |

- **Font**: Inter (substitute for Forma DJR Micro)
- **Card radius**: `16px` · **Button/input radius**: `4px`
- **No pill buttons** — buttons stay sharp
- **Max-width**: 1366px content container
- **Soft Lift shadow**: `0 2px 8px rgba(26,26,26,0.08)`

---

## Layout

```
┌─────────────────────────────────────────────┐
│  Utility strip (ink background, 6px)         │
│  Nav bar (white, HP logo + title)            │
├─────────────────────────────────────────────┤
│  ┌───────────┐  ┌─────────────────────────┐ │
│  │ Sidebar    │  │ Chat area               │ │
│  │ Topics     │  │  Messages (scroll)      │ │
│  │ History    │  │                         │ │
│  │            │  │  User bubbles (HP Blue) │ │
│  │            │  │  Teacher cards (white)  │ │
│  └───────────┘  ├─────────────────────────┤ │
│                  │ Input bar (sticky bottom)│ │
│                  │  "Ask me anything..."    │ │
├─────────────────────────────────────────────┤
│  Footer (ink background)                     │
└─────────────────────────────────────────────┘
```

### Key UI features

- **User messages**: HP Electric Blue bubbles, right-aligned
- **Teacher messages**: White cards on cloud background, left-aligned, with Ai Suotome label
- **Typing indicator**: Bouncing dots with "Ai Suotome is thinking..." label
- **Sticky input bar**: Always visible at the bottom
- **Code blocks**: Dark (ink) background with monospace font
- **Sidebar**: Topics section + conversation history with HP Electric Blue chevron decoration
- **Responsive**: Collapses to single-column on mobile

---

## What You Will Learn

### SQL (Structured Query Language)
| Concept | The Silly Analogy |
|---------|-------------------|
| **SELECT** | "Shin-chan picking snacks from the fridge" |
| **WHERE** | "Shin-chan hiding from Misae" |
| **COUNT** | "Counting how many times Shin-chan got scolded" |
| **GROUP BY** | "Sorting toys into piles" |
| **ORDER BY** | "Arranging candy from biggest to smallest" |

### Excel (The Magic Grid)
| Concept | The Silly Analogy |
|---------|-------------------|
| **SUM & AVERAGE** | "Adding up Shin-chan's pocket money" |
| **Charts** | "Drawing Shin-chan's face with data" |
| **Sort & Filter** | "Organizing Shin-chan's messy room" |

---

## Files

| File | What It Is |
|------|-----------|
| `pavithrabot.html` | The PavithraBot app — ChatGPT-style chat (open in any browser) |
| `teacher.md` | Ai Suotome — the Shinchan-loving teacher's soul and method |
| `config.example.js` | Template — copy to `config.js` and add your OpenRouter API key |
| `config.js` | Your local API key (ignored by git — never committed) |
| `.gitignore` | Prevents `config.js` from being pushed to GitHub |

---

## What Changed (v3 — Ai Suotome Edition)

- **Rebranded**: Master Thalassos → **Ai Suotome** 🎉
- **New personality**: Shinchan-loving, anime-style, fun energy teacher
- **Dark mode toggle**: HP Ink slab aesthetic
- **Voice input**: Web Speech API microphone button
- **Landing page**: `index.html` with full HP design
- **Export chat**: Download conversations as `.txt`

---

## License

Free for everyone. Share it. Teach someone. Data belongs to all of us. Mata ne~! 🎀
