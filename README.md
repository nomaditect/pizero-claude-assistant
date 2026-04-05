# Pi Zero Claude Assistant

A pocket-sized voice assistant built on a Raspberry Pi Zero 2W and PiSugar 
WhisPlay board, powered by the Anthropic Claude API. Press a button, speak, 
and receive a streamed response on a 1.54" LCD screen.

Developed as a practice-based research artefact for **The Silicon Road** — 
a PhD inquiry into how silicon chip evolution has reshaped domestic space, 
human behaviour, and postcolonial design culture.

---

## What it does

1. Hold the push-to-talk button
2. Speak your question
3. Voice is transcribed via OpenAI Whisper
4. Claude API generates a response and streams it to the screen
5. Optionally speaks the response aloud via TTS

---

## Why it exists

This device is not just a gadget. It is a designed object — an attempt to 
materialise questions about who owns AI, where it lives, and what it looks 
like when intelligence is embedded in humble, affordable hardware.

The Pi Zero costs £15. The WhisPlay board sits on top like a shield. The 
whole thing fits in a pocket. This is deliberately not a smart speaker from 
a tech giant. It is a community-scale, repairable, understandable machine.

As a research artefact it asks: *what happens when the black box opens?*

---

## Hardware

| Component | Purpose |
|---|---|
| Raspberry Pi Zero 2W | Main computer |
| PiSugar WhisPlay board | Screen, mic, speaker, button |
| MicroSD card (16GB+) | Storage |
| PiSugar battery (optional) | Portable power |

---

## Architecture
```
YOU
 │  hold button + speak
 ▼
WHISPLAY BOARD  (mic records voice)
 │
 ▼
PI ZERO 2W  (Python orchestrates)
 │
 │  ── WiFi required ──
 │
 ▼
OPENAI WHISPER  (voice → text)
 │
 ▼
CLAUDE API  (generates response)
 │
 ▼
LCD SCREEN  (streams text in real time)
 └──▶  SPEAKER  (optional TTS)
```

---

## Setup

See [setup guide](docs/setup.md) ← *coming soon*

---

## Research context

**Project:** The Silicon Road  
**Institution:** UCL (target — application 2026)  
**Methodology:** Practice-based PhD  
**Artefact type:** Physical computing / embedded AI  
**Themes:** Postcolonial design, domestic technology, Moore's Law, 
community ownership of AI tools

---

## Credits & References

**Forked and adapted from:**  
[sebastianvkl/pizero-openclaw](https://github.com/sebastianvkl/pizero-openclaw) — MIT License  
Original concept: voice assistant on Pi Zero W + WhisPlay board, powered by OpenClaw/OpenAI.

**Hardware:**  
[PiSugar WhisPlay](https://github.com/PiSugar/whisplay-ai-chatbot) — setup guide and hardware driver

**Key modifications in this fork:**  
- OpenClaw gateway replaced with Anthropic Claude API  
- Documented as a practice-based PhD research artefact

---

## License

MIT# pizero-claude-assistant
"A voice assistant built on Raspberry Pi Zero 2W + WhisPlay, powered by the Claude API — developed as a practice-based research artefact for The Silicon Road PhD."

