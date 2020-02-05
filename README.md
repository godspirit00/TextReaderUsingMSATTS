# Text Reader using Microsoft Azure Neural Text-to-speech
A text reader that uses Microsoft Azure Neural Text-to-speech to synthesize speeches
---------
This project is designed to make English listening audio for English learners in China, but it can also serve other purposes.
Microsoft uses deep neural networks, to create a Text to Speech service makes the voices of computers expressive and nearly indistinguishable from natural spoken voice.
## Features
+ Uses Microsoft Azure Neural Text-to-speech voices to synthesize
+ Partial SSML support, which includes the Microsoft supported tags and a custom `<repeat>` that will repeat the designated text.
+ Tailors the input text to meet the requirements of Microsoft, so that you don't need to do it yourself.
+ Friendly SSML editor. You don't need to type the tags yourself.
+ Dialog Maker to help you transform speaker indicators like "Tony:", "Betty:", etc. to the `<voice>` tags so that these lines will be read by desired voices.
+ Automatically detects lines written in Chinese and have them read by a Chinese voice so that you won't have to manually insert the `<voice>` tags.
+ Optimizes the requests to reduce the cost.
+ Export the speech to WAV files.

## How to use
1. Clone this repo. 
2. Follow the guide in the "Getting started" section of [Microsoft Azure Text to Speech](https://azure.microsoft.com/en-us/services/cognitive-services/text-to-speech/) and obtain your subscription key. Be sure to choose a region that supports neural voices.
3. Edit the HTML file, search for `YOUR_SUBSCRIPTION_KEY` and replace it with your subscription key.
4. Find `YOUR_REGION` and replace it with the region you've chosen, e.g.: `westus` for West US.
5. Enjoy!

This project uses [Microsoft Azure Services](https://azure.microsoft.com/en-us/services/cognitive-services/text-to-speech/), [jQuery](https://www.jquery.com/), [audiobuffer-to-wav.js](https://github.com/Jam3/audiobuffer-to-wav).
