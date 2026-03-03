# 🌙 Luna: AI-Powered Voice Assistant

[cite_start]Luna is an interactive Artificial Intelligence voice assistant designed to streamline daily tasks through natural language processing and voice commands[cite: 21, 31]. [cite_start]Built with a modular Python architecture, Luna integrates the **Google Gemini API** to provide intelligent, context-aware responses and real-time utility[cite: 32, 46].

# Model working

<img width="607" height="353" alt="image" src="https://github.com/user-attachments/assets/790b69cf-b59d-44e1-b325-545cc5e2d660" />

[(https://img.youtube.com/vi/hiymIxdmTxw/maxresdefault.jpg)](https://youtu.be/hiymIxdmTxw)


## 🚀 Key Features

* [cite_start]**Natural Language Understanding:** Processes complex user queries using the `gemini-1.5-flash` model[cite: 128, 296].
* [cite_start]**Voice-Activated Command Center:** Operates on a "wake-word" system (recognizing "Luna") for hands-free interaction[cite: 138, 189].
* [cite_start]**Real-Time Information Retrieval:** Fetches and summarizes the latest news updates via integrated News APIs[cite: 188, 211].
* [cite_start]**Multimedia Control:** Managed local and web-based music playback through a dedicated library[cite: 45, 245].
* [cite_start]**Web Automation:** Quick-access voice commands for launching browsers, YouTube, and Google searches[cite: 105, 108].

## 🛠 Technical Architecture

[cite_start]The system is designed with a focus on modularity and separation of concerns[cite: 41, 42]:

| Module | Responsibility | Technologies |
| :--- | :--- | :--- |
| **Main.py** | [cite_start]Central control unit; handles voice capture and task delegation[cite: 43, 49]. | [cite_start]`speech_recognition`, `pyttsx3` [cite: 66, 68] |
| **Gemini.py** | [cite_start]Interfaces with Generative AI for NLP and query resolution[cite: 46, 280]. | [cite_start]`google.generativeai` [cite: 290] |
| **News.py** | [cite_start]Asynchronous fetching of top headlines[cite: 44, 204]. | [cite_start]`requests`, `NewsAPI` [cite: 207, 212] |
| **music_lib.py** | [cite_start]Manages music mapping and automated web playback[cite: 45, 240]. | [cite_start]`webbrowser` [cite: 249] |


## 💻 Implementation Details

[cite_start]Luna utilizes the **Google Speech Recognition** engine to convert audio input into text[cite: 53, 161]. [cite_start]Commands are then filtered: specific keywords trigger local functions (like playing music), while open-ended questions are routed to the Gemini API for advanced processing[cite: 128, 196].

### Core Logic Flow:
1.  [cite_start]**Listen:** Constant background monitoring for the "Luna" wake-word[cite: 142, 189].
2.  [cite_start]**Process:** Convert speech to text and analyze intent[cite: 36, 195].
3.  [cite_start]**Execute:** Delegate to specific script (News, Music, or Gemini)[cite: 59].
4.  [cite_start]**Respond:** Provide audio feedback via the `pyttsx3` text-to-speech engine[cite: 80, 84].

## 🛰 Strategic Value for SpaceTS
This project demonstrates proficiency in building **Human-Machine Interfaces (HMI)**. The ability to create responsive, voice-controlled systems that integrate multiple APIs is essential for developing hands-free diagnostic tools or interactive AI assistants within high-complexity aerospace environments.

---
**Developed by:** Himanshu Raj  
