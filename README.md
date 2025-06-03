This repository contains various notebooks and scripts to generate videos using AI. There are several different workflows presented, in the increasing order of complexity. In each case, we use an LLM (DeepSeekV3), an image generator (Flux/ Stability) and a text-to-speech model (Kokoro). The LLM generates the script and image prompts, which are used by the TTS and image generator, everything is finally put together. Difference is in how the LLM is being used

Videos generated using these notebooks/ scripts are uploaded here:
https://www.youtube.com/@Tales_from_thePast
  
- ************************************** WorkFlow_1: Simple LLM *****************************************
- File: notebooks/ai-video-generator-DeepSeek-Stability-Kokoro.ipynb :
- Only uses the existing "knowledge" of the LLM, nothing additional
- Fine for generic well-known topics and shorter (<5 minute) videos
- ********************************** WorkFlow_2: LLM + wikipedia article *******************************
- File: notebooks/ai-video-generation_with_wiki-DeepSeek-Flux-Kokoro.ipynb :
- Includes a wikipedia article as an additional resource
- As the entire video (scripts + image prompts) is generated in one go, the length is limited by the maximum output tokens of the LLM
- Can create videos of length 10 minutes max
