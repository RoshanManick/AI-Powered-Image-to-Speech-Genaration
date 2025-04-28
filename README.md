# Image to Speech GenAI Tool Using LLM 
AI tool that generates an Audio short story based on the context of an uploaded image by prompting a GenAI LLM model, Hugging Face AI models together with LangChain. Deployed on Streamlit.

## Run App with Streamlit Cloud

[Launch App On Streamlit](https://image-to-speech-genai-tool-using-llm.streamlit.app/)

## Approach
An app that uses Hugging Face AI models to generate text from an image, which then generates audio from the text.

Execution is divided into 3 parts:
- **Image to text:**
  an image-to-text transformer model ([Salesforce/blip-image-captioning-base](https://huggingface.co/Salesforce/blip-image-captioning-base)) is used to generate a text scenario based on the on the AI understanding of the image context
- **Story to speech:**
  a text-to-speech transformer model ([espnet/kan-bayashi_ljspeech_vits](https://huggingface.co/espnet/kan-bayashi_ljspeech_vits)) is used to convert the generated short story into a voice-narrated audio file
- A user interface is built using streamlit to enable uploading the image and playing the audio file
  


## Requirements

- os
- python-dotenv
- transformers
- torch
- langchain
- llama 
- requests
- streamlit
  
