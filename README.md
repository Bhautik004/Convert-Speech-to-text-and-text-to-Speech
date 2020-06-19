# Convert-Speech-to-text-and-text-to-Speech
Speech Recognition is an important feature in several applications used such as home automation, artificial intelligence, etc. This article aims to provide an introduction on how to make use of the SpeechRecognition and pyttsx3 library of Python.

step 1
  pip install speechrecognition
 
 step 2
  pip install pyaudio
  
The PyAudio library serves as a cross-platform Input-Output module and provides bindings with PortAudio. PyAudio enables the user to record and play the audio files irrespective of the platform i.e. it is completely platform-independent.


Understanding Python speech to text conversion using SpeechRecognition module

Step 1: Import the necessary library/module

In the process of conversion of speech to text using SpeechRecognition module, we will have to import the same in our program so as to avail all the functions defined under the module/library.

step 1: import speech_recognition

Step 2: Initialize the Speech Recognizer

variable = speech_recognition.Recognizer()

In order to take the input in the audio format and recognize the sound, it is necessary for us to initialize the recognizer to recognize the audio/voice.

Step 3: Set the source of input audio/voice

The input to the speechrecognition module is of two types:

Pre-recorded audio file
Voice input through default Microphone

with SRG.Microphone() as source

In the above statement, the input to our function is directly recorded through the default microphone. Thus, the Microphone() object is being used to fetch the audio from the microphone.

Note: We need to install the PyAudio module in order to accept the input in audio format from the default microphone.

If you want to convert a pre-recorded audio file to text, we need to follow the following statement:

with SRG.AudioFile(name of the audio file) as source

Step 4: Define the time limit for recording the audio from the microphone.

The record() method is used to set the source of the input and the time for which the microphone needs to accept and record the input audio.

record(source, duration)

source: Defines the source of input such as audio file, input from microphone, etc.
duration: The time period (in seconds) for which the microphone would be active and accept the input voice from the user.

Step 5: Convert the speech to text using a search engine or an API

The record() function accepts the voice from the user and uploads the same to the speech recognition engine such as google voice recognition engine for speech recognition. It is mandatory for the system to stay connected to the Internet in order to use the google recognition engine.

The recognize_google() function recognizes the input voice passed to it as a parameter and returns it in the text form. If the user wishes to use any other language for speech recognition like Spanish, Japanese, etc, will need to pass the language as a parameter to the function.
  

If any quey to  contact me on 2000bhautikpatel@gmail.com
