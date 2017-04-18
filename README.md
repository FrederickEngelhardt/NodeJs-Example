# Node.js Speech Translation Sample App

The sample illustrates how to use two methods supported in the Microsoft Translator Speech Translation API:

1. Calling ~/languages to get the list of supported languages for speech, text and text-to-speech.
2. Calling ~/speech/translate to get the recognition and translation of an audio file. The audio file is in PCM 16-bit, 16 kHz, mono WAV format (with header).

## Instructions

The sample requires a subscription with Microsoft Translator Speech Translation API, which is part of Microsoft Azure Cognitive Services. Visit the [Speech Translation API documentation page](http://docs.microsofttranslator.com/speech-translate.html) for steps about getting a subscription.

To run the sample:

1. First execute `npm install` to get the package dependencies.
2. Edit `app.js` and enter your Azure Cognitive Services subscription key for Microsoft Translator Speech Translation API:
```
var azureClientSecret = '[subscription secret key]';
```
3. Run by executing `node app.js`

If you want to change the audio file, change the line:
``` 
var file = 'helloworld.wav';
```

## Dependencies
request, stream-buffers, websocket
