# Fusion Flow - Multimodal Chatbot for People with Aphasia

A multimodal chatbot that supports text, audio, video and click inputs to support people with Aphasia or any other communication disabilities to navigate within a website.
The project collaborates with the La Trobe University's Research Centre for Data Analytics and Cognition in Australia.

- <b>Project Supervisors</b>
    1. Dr. Uthayasanker Thayasivam
    2. Prof. Damminda Alahakoon
    3. Dr. Achini Adikari
    4. Mr. Nuwan Pallewela
- <b>Contributors</b>
    1. R.L.A. Sanduni Ayesha
    2. L.B.H.M. Vijayarathna
    3. N.P.A. Vithanage

## Summary

Chatbots have become a trending topic with emerging platforms like ChatGPT, Gemini, and Copilot, for conversation assistance. Current chatbots mainly focus on the general public assuming a natural flow of conversation. However, there is a need for a chatbot that supports people with various communication disabilities. This application fills this gap by offering a novel technique for a chatbot that assists people with aphasia, a condition characterised by difficulties with language. 

Aphasia is a neurological disorder affecting the language and communication abilities of people who have suffered from a stroke, traumatic brain injury, or other neurological conditions. Individuals with aphasia often experience difficulties in,
- Speaking
- Understanding spoken language
- Reading
- Writing


We propose a multi-modal chatbot that is customised and designed to assist users with communication disabilities in navigating a website. Unlike typical chatbots, which rely on one form of communication, our architecture combines multiple modalities to improve comprehension and promote effective communication for people with aphasia. We focus on gathering multimodal inputs by recognising and combining user intents from diverse sources. Using Txtai, an all-in-one embedding database for semantic search improves our chatbot’s capacity to process various inputs efficiently. We leverage specialised models like Whisper for audio transcription and MediaPipe Gesture Recognizer for gesture detection to enhance user interactions. We propose that this new approach will make communication more accessible and inclusive for individuals with Aphasia.

  ## Description
  
The application is developed as a WordPress Plugin as it was developed to be integrated with a WordPress website. The [setup process](https://github.com/fusion-flow/.github/edit/main/profile/README.md#setup-documentation) of the application is also mentioned herewith. The [plugin code](https://github.com/fusion-flow/wordpress-site-plugin) and the [flask backend](https://github.com/fusion-flow/flask-backend) code repositories are also included in the project. 

This application mainly gets inputs from 4 modalities, 
- Text
- Audio
- Video (Gesture recognition)
- Clicks

Here the text data is processed by a whisper base [transcription model](https://github.com/fusion-flow/transcription) to get the transcribed text and sent for intent classification along with the text input. These text inputs would be separately classified into the intents using [txtai](https://github.com/neuml/txtai). Based on the classified inputs, an intent would be defined for each modality. The gestures of the users will also be used to detect the shown gesture using a [gesture recognition model](https://github.com/fusion-flow/gesture-recognizer-model). The fusion component will fuse all the inputs from multiple modalities and give the most suitable intent to the dialog manager which would generate the customized response to the user. 

### Architecture Diagram
<img src="https://github.com/fusion-flow/.github/assets/79503916/cd6f3e74-aed9-4396-ab0a-c777bffa18de" width="500" />

### Setup Documentation

You can find the documentation to setup the application by following the [process](https://github.com/fusion-flow/wordpress-site-plugin/tree/main#wordpress-site-local-setup-guide).
All the relevant repositories are included in this project for your easy access.

### Code of Conduct

Please read our code of [conduct document here](https://github.com/aaivu/aaivu-introduction/blob/master/docs/code_of_conduct.md).
<!--

![Chatbot]![Multimodality]![Intent Classification]![Aphasia]![Communication Disabilities]

![Architecture Diagram](https://github.com/fusion-flow/.github/assets/79503916/8a1d3337-d706-42f7-8826-aa8cd3320adf)
**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->


