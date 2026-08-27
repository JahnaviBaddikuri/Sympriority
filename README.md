# Sympriority
An intelligent patient triage application that accepts voice input with multilingual support, enabling easy symptom reporting for diverse users. 

The system analyzes inputs using AI to classify risk levels (Low, Moderate, High, Critical) and generates a priority score.

It then provides real-time clinical insights and recommended actions, guiding patients on whether to seek immediate medical care or follow self-care measures.

## Tools & Technologies

- <b>Speech to Text integration</b> – openai/whisper-medium
- <b>Triage LLM</b> – mistralai/Ministral-3-3B-Instruct-2512
- <b>Gradio</b>  – Used to build an interactive web interface for voice/text input and real-time output display
- <b>Backend</b> - Python
- <b>Frontend</b> – HTML CSS
- <b>Runtime</b> – Google Colob (free tier)
- <b>GPU</b> – NVIDIA T4 – 15 GB VRAM

## Why these models

### Whisper (medium)
- Optimal accuracy-to-efficiency balance for multilingual speech recognition on limited GPU resources
- Achieves ~5% WER on English while reliably handling Hindi, Tamil, and Telugu with built-in translation
  
### Ministral-3B (Instruct)
- Largest instruction-tuned LLM that fits on a T4 GPU alongside Whisper Apache 2.0 licensed (fully open, no access restrictions)
- Strong at structured JSON generation, enabling consistent and reliable triage outputs

## UI / Output Screenshots
<img width="917" height="525" alt="image" src="https://github.com/user-attachments/assets/75a62aec-1857-4aaf-9e73-6a269b6b6948" />
<br>
<img width="933" height="535" alt="image" src="https://github.com/user-attachments/assets/ff5c1ebc-deb6-4ea9-bd6d-527625947c4e" />


## Conclusion

Built a fully functional end-to-end AI triage system running entirely on free infrastructure (Google Colab T4 GPU) 

Seamlessly integrated Whisper (ASR) + Ministral-3B (LLM) into a single intelligent pipeline 

Generates a 6-section structured clinical triage card, comparable to a trained triage nurse’s assessment 

Supports multilingual input (Hindi, Tamil, Telugu, English) with consistent, high-quality output 



