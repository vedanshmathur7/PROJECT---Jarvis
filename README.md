# JARVIS - Voice-Activated Virtual Assistant

**Jarvis** is a voice-activated virtual assistant designed to enhance productivity and entertainment by performing tasks such as web browsing, playing music, fetching the latest news, and responding to user queries. Powered by OpenAI's GPT-3.5-turbo model, Jarvis provides a seamless and intelligent virtual assistant experience similar to Alexa or Google Assistant.

## 🚀 Features

### 1. **Voice Recognition**
   - Utilizes the `speech_recognition` library to listen for and recognize voice commands.
   - Activates upon detecting the wake word **"Jarvis"** for hands-free interaction.

### 2. **Text-to-Speech (TTS)**
   - Converts text responses into speech using `pyttsx3` for offline TTS.
   - Optionally uses `gTTS` (Google Text-to-Speech) combined with `pygame` for clear voice playback.

### 3. **Web Browsing**
   - Opens popular websites such as Google, Facebook, YouTube, and LinkedIn with simple voice commands.

### 4. **Music Playback**
   - Interfaces with a custom `musicLibrary` module to play songs via web links or a predefined library.

### 5. **News Fetching**
   - Fetches and reads the latest news headlines using the [NewsAPI](https://newsapi.org/).

### 6. **OpenAI Integration**
   - Handles complex queries and generates intelligent responses powered by OpenAI's GPT-3.5-turbo model.
   - Acts as a general-purpose virtual assistant capable of holding conversations, answering questions, and assisting with various tasks.

---

## 🛠️ Workflow

1. **Initialization**
   - Greets the user with "Initializing Jarvis..." upon startup.

2. **Wake Word Detection**
   - Continuously listens for the wake word **"Jarvis"** to activate.

3. **Command Processing**
   - Processes recognized commands to determine the appropriate action:
     - **Open websites** like Google or YouTube.
     - **Play music** from a predefined library or links.
     - **Fetch the latest news**.
     - **Answer queries** using OpenAI integration.

4. **Speech Output**
   - Provides spoken responses using the `speak` function, leveraging `pyttsx3` or `gTTS`.

---

## 📚 Libraries Used

This project makes use of the following Python libraries:

- **`speech_recognition`**: For voice command recognition.
- **`webbrowser`**: To open websites programmatically.
- **`pyttsx3`**: For offline text-to-speech conversion.
- **`musicLibrary`**: Custom module for managing and playing music.
- **`requests`**: For fetching news and making API calls.
- **`openai`**: For integrating GPT-3.5-turbo and generating intelligent responses.
- **`gTTS`**: For online text-to-speech conversion.
- **`pygame`**: To play audio generated by `gTTS`.
- **`os`**: For interacting with the operating system.

---

## 🔧 How It Works

1. Jarvis listens continuously for the wake word **"Jarvis"**.
2. Once activated, it acknowledges with a simple "Ya" and waits for the user's command.
3. Based on the command, it can:
   - Open websites in the default browser.
   - Play songs from a music library or web links.
   - Fetch and read out the latest news headlines.
   - Generate intelligent responses for general questions using OpenAI.
4. Provides voice responses to maintain a conversational experience.

---

## 🚀 Getting Started

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/yourusername/jarvis-virtual-assistant.git
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Add your API keys:
   - **NewsAPI**: Add your NewsAPI key in the relevant section of the script.
   - **OpenAI**: Add your OpenAI API key for GPT-3.5-turbo integration.

4. Run the program:
   ```bash
   python jarvis.py
   ```

---

## 🛠️ Future Enhancements

- Integration with smart home devices (e.g., IoT).
- Support for additional languages in speech recognition and TTS.
- Advanced task scheduling and reminders.
- Enhanced GUI for better accessibility.

---

## 🤝 Contributing

Contributions are welcome! If you have ideas to improve Jarvis or would like to report a bug, feel free to create an issue or submit a pull request.

---
