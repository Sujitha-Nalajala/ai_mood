  # 🌙 MoodSpace — AI-Powered Emotional Companion

> *Feel. Adapt. Thrive.*

MoodSpace is an interactive, emotion-aware website that detects your mood from natural text and dynamically adapts its entire interface — colors, animations, and personalized recommendations — to match how you're feeling.

**Built by Sai Sujitha Nalajala**

---

## ✨ Live Demo

🔗 [View Live Site](https://aimoodbysujitha.netlify.app)

---

## 🧠 What It Does

You open the site and write:

> *"I feel overwhelmed and can't focus today."*

MoodSpace instantly:
- Detects your mood as **Anxious**
- Shifts the entire UI to a calmer purple theme
- Activates **Focus Mode** to reduce visual noise
- Offers 3 personalized activities:
  - 🌬 2-minute breathing reset
  - 📓 Guided journal prompts
  - ✅ Tiny action plan

---

## 🎯 Features

### Core
- **AI Mood Detection** — Smart local classifier using lexicon scoring, negation detection, intensifier weighting, emoji signals, and sentence-level patterns. No API key required.
- **Quick Mood Picker** — Tap a feeling directly: Joyful, Calm, Anxious, Energetic, Sad, or Focused
- **Dynamic Theming** — Each mood triggers a unique full-page color palette, background orbs, and glow effects
- **Confidence Score** — Visual bar showing how strongly your text matched the detected mood

### Activities (per mood)
| Activity | Description |
|----------|-------------|
| 🌬 Breathing Reset | Animated 4-2-4 breathing exercise with countdown and cycle tracker |
| 📓 Journal Prompts | 3 mood-specific reflective prompts with a free-write area |
| ✅ Tiny Action Plan | 3-step mood-tailored checklist with tap-to-complete |
| 💛 Motivation | Curated quotes + personalized affirmations for your mood |

### Extra
- **Focus Mode Banner** — Auto-activates for anxious/sad moods to reduce overwhelm
- **Mood History** — Last 6 moods saved locally with timestamps
- **Mini Bar Chart** — Visual trend of your mood over time
- **Day Streak Tracker** — Encourages daily check-ins
- **Custom Cursor** — Smooth animated cursor that follows your pointer
- **No backend, no account, no API key** — 100% client-side, privacy-first

---

## 🛠 Tech Stack

| Layer | Technology |
|-------|-----------|
| Frontend | Vanilla HTML, CSS, JavaScript |
| Mood Classification | Custom local NLP classifier (no API) |
| Storage | `localStorage` (browser-native) |
| Fonts | Cormorant Garamond, DM Mono, Cabinet Grotesk |
| Hosting | GitHub Pages |

---

## 📁 Project Structure

```
moodspace/
│
└── index.html        # Entire app — self-contained single file
```

Everything lives in one file: styles, classifier logic, activity content, history, and animations.

---

## 🚀 Running Locally

No installation needed. Just:

1. Download `index.html`
2. Double-click to open in any browser
3. That's it ✦

---

## 🧩 How the Mood Classifier Works

No API or server involved. The classifier runs entirely in the browser:

1. **Lexicon Scoring** — 30–40 keywords/phrases per mood, each with a weight
2. **Negation Detection** — Catches "I'm *not* happy" and inverts the signal
3. **Intensifier Boosting** — "Very anxious" scores higher than just "anxious"
4. **Multi-word Phrases** — "can't focus", "in the zone", "fired up" score extra
5. **Emoji Signals** — Emotional emojis contribute to mood scores
6. **Sentence Patterns** — Regex matches like "I feel so…" or "I can't stop…"
7. **Punctuation Cues** — Multiple `!` boosts joyful/energetic, `?` nudges anxious
8. **Confidence Calculation** — Based on how dominant the top mood score is vs others

---

## 📸 Mood Themes

| Mood | Theme Color | Trigger Words |
|------|-------------|---------------|
| 😌 Calm | Cool blue | peaceful, relaxed, okay, grounded |
| 😄 Joyful | Fresh green | happy, excited, amazing, grateful |
| 😰 Anxious | Deep purple | overwhelmed, stressed, worried, panic |
| ⚡ Energetic | Warm orange | motivated, ready, fired up, pumped |
| 🌧 Sad | Muted slate | sad, empty, tired, lonely |
| 🎯 Focused | Vivid green | focused, in the zone, determined |

---

## 💼 Resume Description

> Built an AI-powered interactive website that detects user mood from free-text input using a custom local NLP classifier and dynamically adapts the entire interface — including theme, animations, and personalized recommendations — in real time. Implemented state-driven UI with 6 mood themes, 4 activity modules (breathing, journaling, action planning, motivation), mood history with localStorage persistence, and a confidence scoring system. Fully client-side: no API key, no backend, no account required.

---

## 🌱 Future Improvements

- [ ] Voice input for mood detection
- [ ] Mood trend charts over weeks/months
- [ ] Export journal entries as PDF
- [ ] Spotify/YouTube integration for mood-matched music
- [ ] PWA support for offline use and home screen install
- [ ] Dark/light mode toggle
- [ ] Shareable mood cards

---

## 📄 License

MIT License — free to use, modify, and share.

---

*Made with intentionality and care by **Sai Sujitha Nalajala***
