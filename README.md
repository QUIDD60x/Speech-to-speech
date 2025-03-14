# Speech to Speech : Azure TTS version
## A program already built into chatGPT, using chatGPT.
---
## How it works/Why I made this
This program essentially allows you to "speak" with a chatbot, and allows them to speak back. The system works as follows:

1. You speak into your microphone while recording (which will save the recording as a .wav).
2. OpenAIs Whisper translates that recording into text.
3. That translation is sent to your AI API (you will need your own).
4. The response is collected, then spoken out loud (using either PYTTSX3 or Azure's TTS API, depending on your model you want).

And for convenience, the text input + output is collected in a local text file, and the recording is saved (until rewritten by the next input).

This program is best suited for those who find themselves asking for little bits of help while working, something I noticed in myself quite some time ago. 

**THIS VERSION REQUIRES AN AZURE TTS SUBSCRIPTION AND AN API KEY!** This version sounds SIGNIFICANTLY better and is best suited for those who either (1) already have an Azure subscription and don't mind adding on, or (2) plan on using this program constantly.

***
## Quickstart

### Dependencies (for the non-azure TTS model):

* tkinter
* numpy
* openAI
* speechrecognition
* sounddevice
* keyboard
* pyttsx3

You can paste `pip install openai speechrecognition sounddevice numpy keyboard pyttsx3 tkinter` to install all of these immediately.

### How to use:

Firstly You'll need your own ChatGPT API key, and an Azure TTS API key. I explain it a bit more in the script, but you can either add it as an enviromental variable or specify it in the marked variable.

After that, simply install all dependencies and run it in your command line interface.

For any more help check the wiki, or leave me a message on discord (quidd60x).
