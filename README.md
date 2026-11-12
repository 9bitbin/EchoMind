# 🎭 EchoMind: Emotional Voice AI Experience (Tentative Idea Project.) 

**Created by:** Himal & Hammid  
**Project Goal:** An interactive LLM-powered experience featuring real-time voice interaction, emotional emulation, and dynamic reactive behaviors.

---

## 🌟 What is EchoMind?

**EchoMind** is an interactive, voice-first artificial intelligence experience. Unlike traditional virtual assistants like Siri or Alexa—which sound flat, robotic, and neutral—EchoMind feels like talking to a real persona with moods, feelings, and evolving reactions.

When you speak to EchoMind:
1. **It Listens to How You Say It:** It doesn’t just transcribe your words; it detects your tone, energy, and mood.
2. **It Thinks & Feels:** It processes your input through an internal "emotion engine" that shifts its dynamic mood state (e.g., curious, empathetic, defensive, excited).
3. **It Responds with Voice & Expression:** It speaks back to you in real-time, matching its voice inflection, pitch, and pacing to its current emotional state.

---

## 🚀 Key Features

* 🎙️ **Natural Voice Interaction:** Speak directly to the AI—no typing required.
* 🧠 **Emotional Emulation:** The AI possesses an evolving mood matrix that changes based on how you treat it.
* 🎭 **Dynamic Tone Adjustments:** The AI’s voice tone dynamically alters (happy, concerned, sarcastic, warm) to match its internal state.
* 🎯 **Gamified Relationships:** How you interact changes your rapport score, unlocking different dialogue branches and story outcomes.

---

## 🏗️ Technical Architecture Framework

Below is the simple step-by-step pipeline showing how a user's voice input travels through the system to produce an emotionally aware vocal response.

```
+------------------+      +-----------------------+      +-------------------------+
|   1. USER VOICE  | ---> |  2. EAR & MOOD DETECT | ---> |  3. EMOTION CORE (LLM)  |
|  Audio input     |      |  Speech-to-Text (STT) |      |  System Prompt + State  |
|  via Microphone  |      |  + Sentiment Analysis |      |  Mood: [Excited/Anxious]|
+------------------+      +-----------------------+      +-------------------------+
                                                                      |
                                                                      v
+------------------+      +-----------------------+      +-------------------------+
|  6. USER HEARS   | <--- |  5. EXPRESSIVE VOICE  | <--- |   4. DECISION ENGINE    |
|  Emotionally     |      |  Text-to-Speech (TTS) |      |  Chooses dialogue and   |
|  matched audio   |      |  with SSML Tone Tags  |      |  updates rapport state  |
+------------------+      +-----------------------+      +-------------------------+
```

---

## ⚙️ How the 4-Layer Framework Works

To make this complex system easy to understand, we split the architecture into four simple layers:

### Layer 1: Perception (The Ears)
* **Speech-to-Text (STT):** Converts your voice into written text in milliseconds.
* **Acoustic Sentiment Engine:** Analyzes audio cues like loudness, speech rate, and pitch variation to detect emotional cues (e.g., yelling vs. whispering).

### Layer 2: The Emotion Engine (The Heart)
* **Mood State Machine:** Maintains tracking variables for core emotional vectors:
  * `Valence` (Positive vs. Negative mood)
  * `Arousal` (High energy vs. Low energy)
  * `Trust / Rapport` (User relationship score)
* **Contextual Memory:** Remembers how past interactions made the AI feel during your conversation.

### Layer 3: Language & Logic (The Brain)
* **Large Language Model (LLM):** Receives the user's text, acoustic sentiment, and the AI’s current mood variables inside a hidden system prompt.
* **Output Generation:** Generates a human-like response while specifying emotion tags (e.g., `[mood: apologetic]`, `[tone: hesitant]`).

### Layer 4: Expressive Speech (The Voice)
* **Emotional Text-to-Speech (TTS):** Uses advanced voice synthesis engines to translate response text into lifelike speech.
* **SSML / Emotion Tags:** Adjusts cadence, breathiness, pitch shifts, and pauses so the voice authentically matches the generated emotion.

---

## 🎮 How to Play / Run the Experience

### Prerequisites
* Microphone and Speakers / Headphones
* Python 3.10+
* API Keys for:
  * Speech Processing (e.g., Deepgram / Whisper)
  * LLM Provider (e.g., OpenAI / Anthropic / Gemini API)
  * Voice Generation (e.g., ElevenLabs / Azure Speech)

### Quickstart Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/himal-and-hammid/echomind-experience.git
   cd echomind-experience
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set environment variables (`.env`):**
   ```env
   LLM_API_KEY=your_llm_api_key
   VOICE_API_KEY=your_voice_api_key
   ```

4. **Launch the experience:**
   ```bash
   python main.py
   ```

---

## 👥 Credits & Roles

* **Himal:** .
* **Hamid:**
* what will be done: Systems Lead & Emotion Engine Architect (LLM Integration, Mood Logic, Prompt Engineering) Audio Pipeline & Voice Synthesis Lead (STT/TTS Latency Optimization, Acoustic Analysis).

---

## 📄 License
This project is licensed under the MIT License - see the `LICENSE` file for details.
