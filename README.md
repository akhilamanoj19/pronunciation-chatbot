

# 🗣️ Pronunciation Chat Bot

A web-based chatbot that helps users hear the correct pronunciation of words in different languages using an intuitive UI and a Flask-powered backend. Built by **Karthik SN** and **Akhila Manoj N**.

## 🔍 Features

- 🔐 **User Authentication**: Sign up and log in to access personalized features.
- 💬 **Chat Interface**: Enter words, get pronunciations, and play audio directly in the browser.
- 🎧 **Audio Pronunciation**: Leverages Google Text-to-Speech (gTTS) to generate accurate word pronunciations.
- 🕓 **Timestamps**: All messages are timestamped for clarity.
- 💾 **Word History**: Logged-in users can view their previously searched words.
- 🌓 **Theme Toggle**: Switch between light and dark mode (saved using `localStorage`).
- 🧠 **Smart Suggestions**: Real-time word suggestions from an external API.

## 🧱 Tech Stack

### 🔹 Frontend
- **HTML & CSS**: Responsive layout with gradient backgrounds and modern UI.
- **JavaScript**: Handles input, API calls, and dynamic UI updates.

### 🔹 Backend
- **Python Flask**: REST API that handles pronunciation logic.
- **gTTS (Google Text-to-Speech)**: Converts input text to audio.
- **Base64 Encoding**: Audio is sent as Base64 for seamless browser playback.

## 🔁 API Overview

### POST `/pronounce`
**Request:**
```json
{
  "word": "hello",
  "language": "en"
}
```

**Response:**
```json
{
  "word": "hello",
  "status": "success",
  "audio": "base64-encoded-audio-string",
  "language": "en"
}
```

## 📌 Future Improvements

- Improve pronunciation accuracy
- Add support for more languages and accents
- Enhance UI/UX for accessibility and responsiveness



---
