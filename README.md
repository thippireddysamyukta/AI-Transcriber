
   gradio
   google-genai
   
   # 🎤 AI Transcriber

An audio transcription tool powered by Google Gemini and Gradio.
Records voice from your microphone and transcribes it exactly as spoken, including punctuation — no summarization, just accurate speech-to-text.

## Features
- Record audio directly from your microphone
- Accurate, verbatim transcription using Gemini
- Preserves punctuation and phrasing
- Simple, clean Gradio web interface

## Tech Stack
- Python
- Google Gemini API (gemini-2.5-flash)
- Gradio

## Setup
```bash
pip install -r requirements.txt
```
Set your Gemini API key as an environment variable (recommended over hardcoding it):
```python
import os
client = genai.Client(api_key=os.getenv("GEMINI_API_KEY"))
```
Then run:
```bash
export GEMINI_API_KEY="your_api_key_here"
```

## Usage
```bash
python transcriber.py
```
1. Click the microphone to record your voice
2. Click "Transcribe"
3. View the exact transcript in the output box

## License
MIT
