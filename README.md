# Aarogya Saathi 🩺

**Your AI care companion — turning hospital discharge summaries into care a family can actually follow.**

Built for **Innovator's League 2026** (Healthcare domain) — *Discharge Instruction Translator* problem statement.

> **Others translate. We verify the patient understood it.**

---

## The Problem

When a patient leaves an Indian hospital, they receive a discharge summary — a dense page of medical English: drug names, dosages, timings, warning signs, follow-up dates. Research shows that while most patients *say* they understand their discharge instructions, far fewer can correctly state their diagnosis or plan — and poor after-care understanding is strongly linked to readmissions.

The last document of a hospital stay is written for the file. **Aarogya Saathi rewrites it for the family.**

## What It Does

Upload any discharge summary (paste text or a PDF) and **Nisha**, the AI care companion, converts it into a simple, colour-coded daily checklist:

| Section | Example |
|---|---|
| 🍽 **Diet** | Low salt, low oil · fresh fruits & vegetables |
| 💊 **Medicines** | Aspirin 75 mg — after breakfast · Atorvastatin 40 mg — bedtime |
| ⚠️ **Warning Signs** | Chest pain → return to ER immediately |
| 📅 **Follow-up** | Cardiology OPD in 7 days — carry all reports |

Then the features that make it a companion, not a document:

- **🌐 Three languages** — the entire plan switches between English, हिंदी, and தமிழ்
- **🎙 Fully voice-controlled** — the patient *speaks* ("read my medicines") and Nisha reads the plan aloud; the whole app runs hands-free via the Web Speech API
- **✅ Teach-back quiz** — before the family leaves, Nisha asks three simple questions and verifies the answers. This is the core differentiator: others translate; we verify understanding
- **🔒 100% on-device** — parsing, checklist generation and speech all run inside the browser. No server, no account, no upload. Privacy is the architecture
- **🖨 Print mode** — a take-home sheet for the fridge door

## Try It

The entire app is **one HTML file** — no build, no install, works offline.

1. Open `index.html` in any modern browser (Chrome/Edge recommended for full voice support)
2. Click **Load sample summary** (or upload one of the sample summaries in `samples/`)
3. Press **Generate my checklist** — then switch language, speak to Nisha, take the quiz

*(Hosted on GitHub Pages: enable Pages in repo Settings → your app is live at `https://<username>.github.io/AarogyaSaathi/`)*

## Tech

Single-file vanilla HTML/CSS/JS · pdf.js for PDF extraction · Web Speech API (SpeechSynthesis + SpeechRecognition) for voice · rule-based clinical text parsing with a 4-section classifier · optional live-AI mode (Gemini API) behind a clearly-labelled settings panel — the default pipeline is fully offline.

## Repository Structure

```
index.html                              ← the entire app (open & run)
samples/                                ← demo discharge summaries (cardiac + dengue cases, .txt)
```

📎 **The documentation pack — project report (PDF/DOCX), 5-minute demo script, pitch deck, and the sample summaries as printable PDFs — is attached to the [v1.0 release](https://github.com/selva-009/AarogyaSaathi/releases/tag/v1.0).**

## Team

**[Your Team Name]** — [Member 1] · [Member 2] · [Member 3]

*Submitted to Innovator's League 2026.*

---

*AI-generated guidance in this tool simplifies language already written by the treating doctor — it does not invent medical instructions and is not a substitute for professional medical advice.*
