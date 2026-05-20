# DataAnalysis Teacher — PavithraBot

**Learn SQL and Excel through conversation. ChatGPT-style chat with Master Thalassos, powered by OpenRouter AI.**

Hello there. 👋

Do numbers feel overwhelming? Does SQL sound like a foreign language? Do you open Excel and feel lost?

This is for you. Now redesigned as a **ChatGPT-style conversational AI** with the **HP Design System**.

---

## Meet Your Teacher: Master Thalassos

I have been teaching data for **1,247 years**. I taught merchants in Alexandria, accountants in Beijing, and clerks in Victorian London. Now I am here for you.

I do not use big words. I do not rush. I use **stories and pictures** — because that is how humans learn.

> *"A database table is like a filing cabinet. SELECT opens the drawer. WHERE finds the right card."*

---

## AI-Powered Conversational Chat

PavithraBot is now a **ChatGPT-style chat interface**. Every message you send is answered by **OpenRouter AI** (Mistral 7B Instruct) — no more scripted exercises or practice cards. Just you, your questions, and a 1,247-year-old teacher who responds with warmth, analogies, and patience.

### How it works

1. **Type any question** about SQL or Excel in the chat input
2. **Master Thalassos responds** with an AI-generated answer, complete with analogies and code examples
3. **Click a topic** in the sidebar to switch context — the teacher tailors responses to that topic
4. **Conversation history** is maintained for context (last 10 messages)
5. **Fallback responses** kick in if OpenRouter is unavailable — the teacher still responds from built-in knowledge

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
- **Teacher messages**: White cards on cloud background, left-aligned, with Master Thalassos label
- **Typing indicator**: Bouncing dots with "Master Thalassos is thinking" label
- **Sticky input bar**: Always visible at the bottom
- **Code blocks**: Dark (ink) background with monospace font
- **Sidebar**: Topics section + conversation history with HP Electric Blue chevron decoration
- **Responsive**: Collapses to single-column on mobile

---

## What You Will Learn

### SQL (Structured Query Language)
| Concept | The Simple Idea |
|---------|----------------|
| **SELECT** | "Show me everything in this drawer" |
| **WHERE** | "Only show me the vanilla ones" |
| **COUNT** | "How many cards are in this pile?" |
| **GROUP BY** | "Sort these coins into piles" |
| **ORDER BY** | "Line them up by height" |

### Excel (The Magic Grid)
| Concept | The Simple Idea |
|---------|----------------|
| **SUM & AVERAGE** | "The built-in calculator" |
| **Charts** | "Turn numbers into a picture" |
| **Sort & Filter** | "Find what you need, hide the rest" |

---

## Files

| File | What It Is |
|------|-----------|
| `pavithrabot.html` | The PavithraBot app — ChatGPT-style chat (open in any browser) |
| `teacher.md` | Master Thalassos — the teacher's soul and method |
| `config.example.js` | Template — copy to `config.js` and add your OpenRouter API key |
| `config.js` | Your local API key (ignored by git — never committed) |
| `.gitignore` | Prevents `config.js` from being pushed to GitHub |

---

## What Changed (v2)

The original PavithraBot had a Mistral AI design with scripted lessons, practice cards, exercise checking, and a chart sidebar. The new version:

- **ChatGPT-style** conversational interface — every message goes through AI
- **HP Design System** — Electric Blue, Inter font, 4px buttons, 16px cards
- **No more practice cards** — ask questions naturally instead
- **No more check/hint buttons** — the AI teacher guides you
- **No more chart sidebar** — clean two-column layout (sidebar + chat)
- **Typing indicator** with teacher label
- **Sticky input bar** always visible
- **Conversation history** in sidebar
- **Code blocks** with dark (ink) background

---

## License

Free for everyone. Share it. Teach someone. Data belongs to all of us.
