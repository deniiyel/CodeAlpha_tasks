# CodeAlpha AI Projects

A collection of three AI-powered web applications built during the **CodeAlpha** internship. Each project is a self-contained, single-file HTML application — no build tools or dependencies required.

---

##  Projects Overview

| Project | File | Tech Highlights |
|---|---|---|
|  AI Music Generator | `CodeAlpha__Music_Generation_with_AI.html` | LSTM simulation, Web Audio API, MIDI export |
|  Language Translation Tool | `CodeAlpha_Language_Translation_Tool.html` | Claude AI API, Speech Synthesis, 23 languages |
|  FAQ Chatbot | `CodeAplhaChatbot_for_FAQs.html` | TF-IDF, Cosine Similarity, NLP matching |

---

##  Project 1 — AI Music Generator

A browser-based music generation tool that simulates an LSTM neural network trained on musical data, then generates and plays back original note sequences.

### Features
- **LSTM Architecture Visualization** — displays the model layers (Embedding → LSTM 1 → LSTM 2 → Dense → Softmax)
- **Training Simulation** — animated epoch progress bar with live loss/accuracy stats and a loss curve graph
- **4 Genre Modes** — Classical, Jazz, Blues, Pop (each with distinct note patterns and rhythmic styles)
- **Piano Roll Visualizer** — color-coded canvas rendering of the generated note sequence
- **Waveform Preview** — animated waveform display rendered on an HTML5 canvas
- **Web Audio Playback** — plays notes through the browser using the Web Audio API with ADSR envelopes
- **4 Instrument Timbres** — Piano, Synth, Guitar, Strings (each with different oscillator and envelope settings)
- **Adjustable Controls** — tempo (BPM), generation temperature, epoch count
- **MIDI Export** — downloads a valid `.mid` file of the generated composition

### How to Use
1. Select a **Genre** and adjust **Epochs** and **Temperature**
2. Click **Train Model** and wait for training to complete
3. Click **Generate Music** to produce a note sequence
4. Choose an **Instrument** and **BPM**, then click **Play**
5. Optionally click **Download MIDI** to save the output

### Tech Stack
`HTML5 Canvas` · `Web Audio API` · `Vanilla JavaScript` · `MIDI binary encoding`

---

##  Project 2 — Language Translation Tool (LinguaAI)

A clean, professional translation interface powered by the **Claude AI API** (claude-sonnet-4), supporting 23 languages with text-to-speech playback.

### Features
- **AI-Powered Translation** — sends requests to the Anthropic Claude API for accurate, context-aware translations
- **23 Languages** — English, Urdu, Arabic, French, German, Spanish, Italian, Portuguese, Russian, Chinese, Japanese, Korean, Hindi, Turkish, Dutch, Polish, Swedish, Indonesian, Thai, Vietnamese, Persian, Hebrew, Bengali
- **Auto Language Detection** — detects the source language automatically
- **Language Swap** — swap source and target languages (and their text) with one click
- **Text-to-Speech** — listen to both source and translated text using the browser's Speech Synthesis API
- **Copy to Clipboard** — one-click copy of the translated output
- **Character Counter** — tracks input up to the 2,000 character limit
- **Keyboard Shortcut** — `Ctrl+Enter` / `Cmd+Enter` to translate instantly

### How to Use
1. Select source and target languages (or leave source on **Detect Language**)
2. Type or paste text into the left panel
3. Click **Translate →** or press `Ctrl+Enter`
4. Use the ** Listen** buttons to hear either text read aloud
5. Click ** Copy** to copy the translation

### Tech Stack
`Anthropic Claude API` · `Web Speech API` · `Vanilla JavaScript` · `Inter font`

> **Note:** Requires an Anthropic API key configured in the environment to function.

---

## 🤖 Project 3 — FAQ Chatbot

An NLP-powered FAQ assistant that matches user questions to a curated knowledge base using **TF-IDF vectorization** and **cosine similarity** — entirely in-browser, no external API needed.

### Features
- **NLP Matching Engine** — implements TF-IDF (Term Frequency–Inverse Document Frequency) and cosine similarity from scratch in JavaScript
- **3 Topic Domains** — switch between Tech Support, E-Commerce, and Healthcare FAQ databases
- **Confidence Score** — every response shows a match confidence percentage with a color-coded bar (green / yellow / red)
- **Suggested Questions** — clickable quick-start prompts shown on load and on low-confidence responses
- **Typing Indicator** — animated three-dot indicator while the bot "processes" the query
- **Auto-Resize Input** — textarea grows with the message up to a maximum height
- **Keyboard Support** — press `Enter` to send (Shift+Enter for new line)
- **Stopword Filtering** — removes common words before vectorizing to improve match quality

### FAQ Domains
| Domain | Sample Topics |
|---|---|
|  Tech Support | Passwords, internet issues, software updates, cache, 2FA, backups |
|  E-Commerce | Order tracking, returns, payments, promo codes, account issues |
|  Healthcare | Appointments, prescriptions, lab results, insurance, data privacy |

### How to Use
1. Select a **topic** from the tab bar at the top
2. Type a question or click one of the **suggested questions**
3. The bot matches your query against the FAQ database and returns the best answer with a confidence score

### Tech Stack
`TF-IDF` · `Cosine Similarity` · `Vanilla JavaScript` · `No external dependencies`

---

##  Getting Started

All three projects are standalone HTML files. No installation or build step is required.

```bash
# Clone the repository
git clone https://github.com/your-username/codealpha-projects.git

# Open any file directly in your browser
open CodeAlpha__Music_Generation_with_AI.html
open CodeAlpha_Language_Translation_Tool.html
open CodeAplhaChatbot_for_FAQs.html
```

Or simply double-click any `.html` file to open it in your default browser.

>  **For the Translation Tool:** The Claude API call requires a valid Anthropic API key. The key must be available to the frontend environment (configured per the deployment setup).

---

##  Technologies Used

- **Vanilla JavaScript** — all logic written in plain JS, no frameworks
- **HTML5 Canvas** — piano roll, waveform, and loss graph visualizations
- **Web Audio API** — real-time audio synthesis and playback
- **Web Speech API** — text-to-speech for the translation tool
- **Anthropic Claude API** — AI translation backend (`claude-sonnet-4-20250514`)
- **CSS3** — animations, gradients, glassmorphism UI styling

---

##  License

This project was built as part of the **CodeAlpha** internship program. Feel free to use it for learning and reference purposes.

---

*Built with  during the CodeAlpha AI/ML Internship*
