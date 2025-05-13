# Ai-Medical-chatbot
Ai Medical chatbot
🩺 AI Doctor with Vision and Voice
This project is a learning-oriented AI assistant that mimics the behavior of a professional doctor. It accepts voice and image inputs from users and provides medical-like feedback using large language and vision models. The interface is built with Gradio for ease of use.

🔧 Features
🎙️ Voice-to-text conversion using Groq Whisper (via Groq API)

🖼️ Image analysis using LLaMA vision models from Groq

🧠 Intelligent doctor-like responses to both voice and image input

🔊 Text-to-speech using ElevenLabs (or fallback to gTTS)

🧪 Runs locally with a simple Gradio web interface

📁 Project Structure
main.py: Gradio app interface and logic

brain_of_the_doctor.py: Handles image encoding and vision analysis with Groq

voice_of_the_patient.py: Handles voice recording and transcription

voice_of_the_doctor.py: Handles TTS responses

.env: Store environment variables (e.g., GROQ_API_KEY)

🧠 System Prompt
This system simulates a doctor. The model is prompted to:

Diagnose based on uploaded images

Offer brief advice or remedies

Speak naturally, avoiding AI-specific disclaimers or markdown

Example system prompt:

With what I see, I think you have...

🚀 How to Run
Clone this repo

Install dependencies:

bash
Copy code
pip install -r requirements.txt
Set your environment variable:

bash
Copy code
export GROQ_API_KEY=your_groq_api_key_here
Run the app:

bash
Copy code
python main.py
Open the interface in your browser:

cpp
Copy code
http://127.0.0.1:7860
💡 Notes
This is a learning project and not for actual medical use.

You can swap ElevenLabs with gTTS if API key or voice quality is an issue.

Images are encoded as base64 and processed with multimodal Groq models.

🔐 Environment Variables
Variable	Description
GROQ_API_KEY	Your Groq API key
ELEVEN_API_KEY	(Optional) ElevenLabs API key

📝 License
This project is intended for educational use only. Do not use this for real medical diagnostics.
