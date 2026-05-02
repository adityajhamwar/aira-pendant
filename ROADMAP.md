# AIRA Project Roadmap

## Phase 0: Setup & Learn (May–June 2026)
**Goal:** Everything ready for the build sprint after exams.

**Aditya:**
- Order all hardware components.
- Set up GitHub repository, license, README.
- Bookmark essential tutorials (ESP32, Docker, Pipecat).
- Watch one tutorial per day.
- Join relevant Discords/Reddits.
- Scout UCD MakerSpace for TPU filament.

**Shonali:**
- Install Docker, Ollama, whisper.cpp.
- Run Pipecat "hello world" voice agent example.

**Milestone:** All parts in hand. GitHub public.

---

## Phase 1: Hardware Prototyping (Mid-June – Mid-July)
**Goal:** Breadboarded AIRA that streams audio over Wi-Fi.

**Aditya:**
- Session 1: Unbox XIAO, run blink sketch.
- Session 2: Wire INMP441 mic, test I²S audio capture.
- Session 3: Flash Owl firmware, verify Wi-Fi streaming.
- Session 4: Add WS2812B LED, test status colours.
- Session 5: Add tactile button, test push-to-record.
- Session 6: Solder onto perfboard, test battery power.
- Session 7: 3D-print first TPU case, dry fit.

**Shonali:**
- Set up server endpoint for audio, run whisper.cpp.
- Output raw transcript to console.

**Milestone:** Pendant-shaped breadboard that records, streams, and transcribes.

---

## Phase 2: Basic Intelligence (Mid-July – August)
**Goal:** End-to-end voice → summary.

**Aditya:**
- Iterate enclosure (fit, lanyard slot, LED visibility).
- Test pipeline in different noise environments.
- Write user documentation (pairing, charging, LED guide).
- Share demo video on Hackaday.io and GitHub.

**Shonali:**
- Replace simple server with Pipecat pipeline.
- VAD + whisper.cpp → Ollama (llama3.2:1b) → summary.
- Optional: Telegram bot for summaries.

**Milestone:** Speak a sentence, get a summary in seconds. MVP achieved.

---

## Phase 3: Speaker Awareness & Memory (Sept–Oct 2026)
**Goal:** Knows who said what, remembers across sessions.

**Aditya:**
- Test with multiple people, check attribution accuracy.
- Refine design based on real use.
- Prepare "Help Wanted" list for contributors.

**Shonali:**
- Integrate pyannote.audio for diarization.
- Integrate Letta (MemGPT) for persistent memory.
- Set up nightly "dream cycle" memory cleanup.

**Milestone:** Multi-speaker notes with persistent memory.

---

## Phase 4: Learning & Polish (Nov–Dec 2026)
**Goal:** Self-learning loop, first small batch for sale.

**Aditya:**
- Add thumbs-up/down feedback logging.
- Compile 50-example feedback dataset.
- Run test fine-tuning with Unsloth.
- Finalise enclosure for 10-unit batch.
- Launch pre-orders on Tindie.

**Shonali:**
- Build automated feedback → fine-tuning pipeline.
- Polish Open WebUI dashboard.

**Milestone:** Self-improving AIRA. First 10 units ready.

---

## Phase 5: Community & Growth (Early 2027)
**Goal:** Sustainable small-scale production.

**Aditya:**
- Ship first batch, gather feedback.
- Monthly "drop" batches (5–10 units).
- Collaborate with open-source contributors on v2.
- Apply for NovaUCD accelerator / Enterprise Ireland funding.

**Milestone:** AIRA is a recognised name in privacy-AI. Self-sustaining side project.

---

## ⏱️ 1–2 Hour Session Guide

| Session Type | What You Can Do |
| :--- | :--- |
| Building | Solder 2–3 connections, test a sensor, or print one enclosure. |
| Testing | Run the full pipeline 5–10 times with different phrases, note errors. |
| Documenting | Write one section of a build guide or update README with new photos. |
| Learning | Watch one focused tutorial and replicate the steps. |
| Community | Post one devlog, answer one Reddit comment, or triage two GitHub issues. |
