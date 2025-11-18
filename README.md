📌 Overview

JARVIS is a personal voice-controlled AI assistant built in Python.
It can recognize your voice, answer questions using ChatGPT, perform system tasks, take notes, fetch weather updates, define words, open apps/websites, and much more.

This project uses speech recognition, text-to-speech, OpenAI API, Wikipedia, and OpenWeatherMap API.

🚀 Features
✔ Wake-word activation (“Hey Jarvis”)

Listens continuously and activates when you say the wake word.

✔ Voice commands

Open YouTube, Google, Notepad, VS Code

Shut down or restart PC

Tell time & date

✔ AI Chat using GPT

Ask anything and JARVIS replies using OpenAI API.

✔ Notes system

Take notes

Read saved notes

✔ Dictionary meaning

Uses PyDictionary (or GPT fallback) to define words.

✔ Weather updates

Fetches live weather using OpenWeather API.

✔ Play local music

Automatically plays songs from your Music folder.

✔ Face unlock (dummy camera mode)

Activates webcam and shows live feed.

🛠️ Technologies Used
Module	Purpose
speech_recognition	Voice input
pyttsx3	Text-to-speech
openai	GPT responses
wikipedia	Quick summaries
cv2	Face unlock camera window
requests	Weather API calls
PyDictionary	Word meanings
webbrowser	Opening websites
📦 Installation
1. Install Python

Python 3.8+ recommended.

2. Install required libraries

Run:

pip install pyttsx3 SpeechRecognition wikipedia requests PyDictionary openai opencv-python


For microphone support:

pip install pipwin
pipwin install pyaudio

🔑 API Keys Setup
OpenAI API

Replace:

openai.api_key = "YOUR_API_KEY"


with your real key from
https://platform.openai.com/

OpenWeatherMap API

Replace:

api_key = "YOUR_OPENWEATHER_API_KEY"


Get your free key from:
https://openweathermap.org/api

▶ How to Run

Save the full script as jarvis.py

Open terminal in the folder

Run:

python jarvis.py


Wait for the message:
“Say 'Hey Jarvis' to activate me.”

Speak the wake word → JARVIS becomes active.

🎤 Sample Commands

You can say:

"Hey Jarvis, take note"

"What is AI?"

"Define gravity"

"Open YouTube"

"Play music"

"Weather today"

"Tell me the date"

"Face unlock"

"Shutdown the system"

⚠ Known Issues

PyDictionary sometimes fails → use GPT fallback

Wake-word loop may be slow on some microphones

Webcam permission may be required

Ensure stable internet for GPT & Weather API

📌 Future Improvements

GUI Jarvis interface

Real face recognition unlock

Hotword engine (Porcupine / Snowboy)

Android APK version

🤝 Credits

Created by Durgesh Yadav .
Built using Python and OpenAI.