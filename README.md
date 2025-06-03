# AI-Generated Video Workflows

This repository contains a set of notebooks and scripts for generating narrated videos using AI. Each workflow combines an LLM (DeepSeek V3), an image generation model (Flux or Stability), and a text-to-speech model (Kokoro). The LLM generates both the narration script and image prompts; images and audio are synthesized separately and assembled into a video.

Videos created using these workflows are available at:  
https://www.youtube.com/@Tales_from_thePast

## Workflows

### Workflow 1: Basic LLM Generation  
**File**: `notebooks/ai-video-generator-DeepSeek-Stability-Kokoro.ipynb`  
- Uses the LLM without any external sources  
- Suitable for short, general-topic videos (under 5 minutes)  

### Workflow 2: LLM with Wikipedia Source  
**File**: `notebooks/ai-video-generation_with_wiki-DeepSeek-Flux-Kokoro.ipynb`  
- Augments LLM with a Wikipedia article  
- All script and prompts are generated in a single pass  
- Output length constrained by LLM token limits (~10 minutes max)
