# AIRA – Complete Feature List

## 🔒 Always-On Listening & Privacy

- **Wake-word activation ("Hey Aira")**  
  *Why:* Prevents recording unintended private moments.  
  *How:* On-device model listens for wake word, only then streams audio.

- **Physical push-to-talk**  
  *Why:* Tactile, transparent privacy control.  
  *How:* Button directly starts/stops audio capture via GPIO.

- **Voice activity detection with status light**  
  *Why:* Saves battery, shows others when recording is active.  
  *How:* Lightweight model ignores silence; LED glows when speech is captured.

- **Multilingual auto-detection (30+ languages)**  
  *Why:* Works in any language without manual switching.  
  *How:* STT engine detects language from audio, passes code to summariser.

## 👥 Multi-Speaker Awareness

- **Speaker diarization ("who said what")**  
  *Why:* Makes notes usable for meetings and group conversations.  
  *How:* Model separates audio into speaker-labelled chunks before transcription.

- **(Future) Voiceprint recognition**  
  *Why:* Replaces "Speaker 1" with actual names.  
  *How:* Trained voiceprints match speakers in real time, entirely on-device.

## 🧠 Intelligence & Memory

- **Conversation summarisation**  
  *Why:* Raw transcripts are too long; users need short, actionable recaps.  
  *How:* LLM turns multi-speaker transcript into bullet points with extracted tasks.

- **Persistent knowledge graph**  
  *Why:* Remembers key facts across days, not just one conversation.  
  *How:* Facts auto-extracted and stored in structured local memory file.

- **Nightly memory cleanup ("dream cycle")**  
  *Why:* Prevents memory from becoming a cluttered junk drawer.  
  *How:* Scheduled job merges duplicates, archives low-importance data.

## ⚡ Actions & Integration

- **Automatic reminder & task extraction**  
  *Why:* No manual calendar entry needed for spoken promises.  
  *How:* AI outputs structured action objects pushed to user's calendar.

- **User-owned cloud sync**  
  *Why:* Full data ownership without trusting a company server.  
  *How:* User connects their own Nextcloud/Seafile account.

## 📈 Self-Learning & Control

- **Feedback loop (thumbs up/down + edit)**  
  *Why:* Personal AI improves through user corrections.  
  *How:* Each summary rated/edited; corrections saved as training examples.

- **Periodic local fine-tuning**  
  *Why:* Feedback should actively improve the local model.  
  *How:* High-rated examples fine-tune model weekly via Unsloth.

- **Dynamic model routing (local vs. cloud toggle)**  
  *Why:* Full user control over privacy vs. power.  
  *How:* Switch routes requests to local model or user-provided cloud API key.
