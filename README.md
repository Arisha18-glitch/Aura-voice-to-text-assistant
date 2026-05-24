# AURA – Where Voices Come to Life! 🎙️

AURA (Audio Visual Response) is an interactive, voice-responsive system that merges AI-driven speech processing with embedded hardware to create a personalized assistant experience.
<img width="480" height="360" alt="image" src="https://github.com/user-attachments/assets/b383a354-e89b-46be-ac02-60973b1d4803" />

## What It Does

AURA listens to your voice, processes it through OpenAI's Whisper speech recognition model, displays both the input and system response on an LCD screen with an animated face, and speaks back through a speaker module — all powered by Arduino hardware.

## Features

- Real-time voice input via microphone
- Speech-to-text processing using Python Whisper model
- LCD display output with animated facial expressions
- Speaker module for audio responses
- Seamless communication between Python and Arduino over serial

## Tech Stack

- **Hardware:** Arduino Mega, Arduino Nano, TFT LCD 3.5", Speaker Module
- **Software:** Python, OpenAI Whisper, ffmpeg
- **Communication:** Serial (USB) between Python and Arduino
- **Language:** C++ (Arduino), Python

## Project Structure
AURA/
├── TFT_LCD_3.5inch_Arduino_Testing.ino   # Arduino sketch for LCD display and face animation
├── voice_to_arduino.py                    # Python script for voice capture and Whisper processing
## How to Run

1. Upload the `.ino` file to your Arduino using Arduino IDE
2. Install Python dependencies:
```bash
pip install openai-whisper pyserial ffmpeg-python
```
3. Run the Python script:
```bash
python voice_to_arduino.py
```
4. Speak into the microphone — AURA listens, processes, and responds.
