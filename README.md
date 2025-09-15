##  Features

* **Audio Preprocessing** – normalize audio with `pydub` + `ffmpeg`
* **Transcription & Diarization** – convert speech to text and separate speakers
* **Talk Time Ratio** – compare rep vs. customer speaking balance
* **Speech Pace Analysis** – words per minute estimation
* **Interruption & Pause Detection** – conversational flow indicators
* **Sentiment Analysis** – track emotions across the call timeline
* **Question Classification** – open vs. closed questions
* **Named Entity Recognition (NER)** – detect names, orgs, money using spaCy
* **Abstractive Summarization** – Hugging Face summarizer for concise narratives
* **Visualizations** – plots for talk distribution, sentiment trends, word clouds

---

## Project Overview

Built a call analysis pipeline that processes raw audio, transcribes speech, and applies multiple layers of natural language and behavioral analysis to extract meaningful insights from sales conversations.

The pipeline begins with audio preprocessing using **pydub** and **ffmpeg**, ensuring the input is normalized to a consistent format suitable for transcription. Once preprocessed, the audio is passed through a transcription and diarization step to separate speakers and align their contributions. From there, I implemented the `CallAnalyzer` class, which performs various analyses: calculating **talk time ratios** between the sales representative and customer, estimating **speech pace** (words per minute), and detecting **interruptions** and **pauses** that signal conversational dynamics.

For deeper insight, the system applies a Hugging Face **sentiment analysis model** to track how customer and representative emotions evolve throughout the call. Additionally, I classify **open- and closed-ended questions**, helping assess conversational quality. Using **spaCy**, the pipeline extracts key entities such as people, organizations, and monetary values. Finally, a Hugging Face **abstractive summarizer** generates a concise narrative of the call.

This modular design allows for extensibility, better interpretability of sales conversations, and the foundation for future enhancements like scoring or automated coaching feedback.

---

