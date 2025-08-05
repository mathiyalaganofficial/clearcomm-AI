# 🎙️ ClearComm AI  
**Real-Time Accent & Speech Disorder Clarifier**

## 🧠 Overview

**ClearComm AI** is an open-source AI assistant that listens to accented or speech-impaired audio and outputs a clarified version — either as clean text or re-spoken in neutral speech. The goal is to bridge the communication gap for people with strong regional accents, stammering, slurring, dysarthria, or other non-standard speech patterns.

### 🚀 You speak → AI listens → AI outputs clearer version (text or voice)

---

## 💡 Real-World Problem

Many individuals face communication barriers due to non-standard speech:
- Students from rural backgrounds or regional accents
- People with speech disorders like stuttering or slurring
- Elderly or non-native English speakers
- Job seekers struggling in interviews due to unclear speech

Existing STT (Speech-To-Text) systems like Google/Whisper fail in these scenarios, leading to frustration and miscommunication.

---

## 🎯 Project Goals

- 🎤 Accurately transcribe non-standard or impaired speech using Whisper or wav2vec2
- 🔁 Normalize or clarify the speech in real-time using custom logic
- 🔊 Convert the cleaned output into clear, neutral voice using Coqui TTS
- 🖥️ Provide an interactive UI (Streamlit) with mic input and real-time feedback
- 🧪 Compare original vs clarified speech and text side-by-side
- 💻 All tools and models used are **open-source** and **cost-free**

---

## 🛠️ Tech Stack

| Component      | Tools Used                          |
|----------------|-------------------------------------|
| Speech-to-Text | OpenAI Whisper / wav2vec2           |
| TTS            | Coqui TTS or Bark                   |
| Data           | Mozilla Common Voice, UASpeech, TORGO |
| Audio I/O      | pyaudio, sounddevice, torchaudio    |
| Frontend       | Streamlit or Gradio                 |
| ML Frameworks  | PyTorch, Hugging Face Transformers  |

---

## 👥 Team

| Member | Role                          |
|--------|-------------------------------|
| A      | STT / Whisper Fine-tuning     |
| B      | TTS / Synthetic Speech Gen    |
| C      | Streamlit UI / Audio Pipeline |

---

## 📦 Project Structure

```bash
ClearComm-AI/
├── data/                # Datasets / links
├── models/              # Fine-tuned model checkpoints
├── src/
│   ├── stt/             # Whisper/wav2vec2 scripts
│   ├── tts/             # Coqui/Bark modules
│   ├── normalizer/      # Speech clarification logic
│   └── ui/              # Streamlit app
├── requirements.txt     # Python dependencies
└── README.md            # You're here!
