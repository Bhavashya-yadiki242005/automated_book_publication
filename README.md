# Automated Book Publication Project

### Submitted by: Bhavashya Chandra Yadiki

---

## Overview

This project automates the process of fetching book chapters from the web, processing the text using AI, allowing a human review step, and saving multiple versions of the content.  
developed using **Python, Playwright, FastAPI, and ChromaDB** as part of the Agentic AI task assignment.

---

## Features

- **Scraping:** Extract book content and save text with a screenshot.  
- **AI Writer:** Perform basic AI-powered text transformation.  
- **Human-in-the-Loop:** Allows manual editing of AI-generated text.  
- **FastAPI UI:** Web interface to trigger each process step.  
- **Database Versioning:** Store and retrieve different text versions.  

---

## Project Files:
- scrape_and_screenshot.py → Script for scraping chapters
- ai_writer_reviewer.py → Rewrites and processes text
- human_feedback_loop.py → Lets user edit final text
- agentic_api.py → FastAPI endpoints
- db_versioning.py → Saves different versions of text
- chapter1.txt → Raw scraped text
- chapter1_final.txt → Final approved version
- README.md



## API Endpoints
- `/scrape` → Gets a book chapter from the website
- `/ai_writer` → Rewrites the text automatically
- `/human_review` → Lets you edit the text manually
- `/download_final` → Download the final version of the text
- `/voice_command` → Use voice input to control actions
- `/rl_feedback` → Save feedback for improving results



How to Run the Project
Create virtual environment (first time only):
python -m venv venv

Activate environment:
venv\Scripts\activate

Install dependencies:
pip install playwright requests beautifulsoup4 openai chromadb fastapi uvicorn pydantic pyttsx3 SpeechRecognition
python -m playwright install

Run the FastAPI server:
uvicorn agentic_api:app --reload

Open the browser:
http://127.0.0.1:8000/docs


Demo:
A  demo video google drive lunk is included here   showing the full pipeline execution.
LINK:

https://drive.google.com/file/d/1_i9bybzzLvsnVWi7VjMKPuJ1gniJo5hS/view?usp=sharing

screenshots of diffrent steps are avaliable in the screenshots/folder.



How to Run the Project
1. Create virtual environment (first time only):
python -m venv venv

2. Activate environment:
venv\Scripts\activate

3. Install dependencies:
pip install playwright requests beautifulsoup4 openai chromadb fastapi uvicorn pydantic pyttsx3 SpeechRecognition
python -m playwright install

4. Run the FastAPI server:
uvicorn agentic_api:app --reload
5. Open the browser:
http://127.0.0.1:8000/docs

Demo:
A demo video Google Drive link is included here showing the full pipeline execution.
LINK: https://drive.google.com/file/d/1_i9bybzzLvsnVWi7VjMKPuJ1gniJo5hS/view?usp=sharing

Screenshots of different steps are available in the screenshots/ folder.
