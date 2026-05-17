# SPEECH-RECOGNITION-SYSTEM

COMPANY: CODTECH IT SOLUTIONS

NAME: CHAITANYA DODLA

INTERN ID: CTIS8397

DOMAIN: ARTIFICIAL INTELLIGENCE

DURATION: 8 WEEKS

MENTOR: NEELA SANTOSH KUMAR

This project is a Speech Recognition System developed using Python. The main purpose of this project is to convert human speech from an audio file into text automatically using Artificial Intelligence (AI) and Speech Recognition technology. Speech recognition is an important application of Natural Language Processing (NLP) that allows computers to understand and process human voice input. This project helps users easily convert spoken words into written text without manual typing.

For developing and running this project, the main platform used is Google Colab. Google Colab is a cloud-based Python programming environment provided by Google. It allows users to write and execute Python code directly in a web browser without installing software on their computer. Google Colab is very useful for AI and machine learning projects because it provides free CPU and GPU support, making code execution faster and easier.

This project mainly uses two Python libraries:

SpeechRecognition

pydub

The SpeechRecognition library is used to recognize speech and convert audio into text. It supports multiple speech recognition engines, including Google Speech Recognition. The pydub library is used to process and convert audio files from one format to another. In this project, the audio file is converted from .m4a format into .wav format because the SpeechRecognition library works better with WAV audio files.

Before running the project, the required libraries are installed using the following commands:

!pip install SpeechRecognition pydub !apt-get install ffmpeg

The ffmpeg tool is required because pydub uses it to process audio files. After installing the libraries, the Python code imports the required modules and creates a recognizer object using:

recognizer = sr.Recognizer()

The project then loads the audio file named Recording.m4a and converts it into converted.wav using the AudioSegment class from pydub. This conversion step is important for accurate speech processing.

The main function in this project is recognize_speech(). Inside this function, the program reads the converted WAV audio file using sr.AudioFile(). The recognizer records the audio data and sends it to Google’s speech recognition service using:

recognizer.recognize_google(audio_data)
output:

Google Speech Recognition processes the audio and returns the spoken words as text. The recognized text is then displayed on the screen. The project also includes exception handling to manage errors such as unclear audio, internet issues, or unsupported files. This improves the reliability of the application.

This Speech Recognition System has many real-world applications. Students can use it to convert lectures into notes. Journalists can transcribe interviews quickly. Businesses can use it for meeting transcription and customer support systems. It can also be used in virtual assistants, voice-controlled applications, accessibility tools for disabled users, and automated subtitle generation.

This project demonstrates how Python and AI technologies can be used to build a simple and effective speech-to-text system. By using Google Colab, SpeechRecognition, and pydub libraries, developers can easily create voice-processing applications without requiring advanced hardware or deep technical knowledge.

OUTPUT:
