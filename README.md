# Text-To-Speech
REAL-TIME SPEECH TO TEXT TO SPEECH: BUILDING YOUR AI-BASED ALEXA - USING GOOGLE'S gTTS FOR TEXT-TO-SPEECH
Real-time speech to text to speech can be created using OpenAI Whisper and gTTS. For this, the user asks a question by saying a wake word. This is used to identify if the input can be transcribed or not. Also, the voice must have a threshold energy, in a given language for the model to process it.
STEP 1:
User asks a question.
The question is asked through a microphone and the audio is recorded using PythonSpeechRecognition.
 ![image](https://github.com/savithashreem07/Text-To-Speech/assets/157434708/a4c13355-5210-446a-a52d-ce479fdc8120)


STEP 2:
Transcribe the audio to text using OpenAI Whisper
![image](https://github.com/savithashreem07/Text-To-Speech/assets/157434708/8618e9a6-9b83-46ac-815e-1a8888cf0fb3)

 
STEP 3:
The text is processed using OpenAI text completion and the answer is returned as a text.
 ![image](https://github.com/savithashreem07/Text-To-Speech/assets/157434708/30bbf527-9d94-4065-b120-642a9251b3ba)


STEP 4:
Now the text is saved to mp3 file and sent to gTTS to send a voice response.
 ![image](https://github.com/savithashreem07/Text-To-Speech/assets/157434708/e2750bc6-eabd-4235-a006-b37b7b59a914)


All these processes will run simultaneously as separate threads and we have 3 threads in total here.
 ![image](https://github.com/savithashreem07/Text-To-Speech/assets/157434708/31fc4fe9-1ca2-4a3c-bcd2-7a07c1ca04b7)



OUTPUT:
 ![image](https://github.com/savithashreem07/Text-To-Speech/assets/157434708/69fda7a7-eb84-4056-a026-6de093e58043)

This is the entire object from which we are interested in the message content alone which is played as a response to the question asked.
Asking simultaneous questions looks like,
![image](https://github.com/savithashreem07/Text-To-Speech/assets/157434708/13025076-a436-4812-9c12-3fa5d4ad3386)

