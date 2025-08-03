# Automated Book Publication Project

### Submitted by: Bhavashya Chandra Yadiki

---

## Overview

This project automates the process of fetching book chapters from the web, processing the text using AI, allowing a human review step, and saving multiple versions of the content.  
It is developed using **Python, Playwright, FastAPI, and ChromaDB** as part of the Agentic AI task assignment.

---

## Key Features

- **Scraping:** Extract book content and save text with a screenshot.  
- **AI Writer:** Perform basic AI-powered text transformation.  
- **Human-in-the-Loop:** Allows manual editing of AI-generated text.  
- **FastAPI UI:** Web interface to trigger each process step.  
- **Database Versioning:** Store and retrieve different text versions.  

---

## Project Structure
```
automated_book_publication/
│
├── scrape_and_screenshot.py     # Scrapes chapter and takes screenshot
├── ai_writer_reviewer.py        # AI text processing
├── human_feedback_loop.py       # Human review step
├── agentic_api.py               # FastAPI routes
├── db_versioning.py             # Database version control
├── chapter1.txt                 # Scraped text
├── chapter1_spun.txt            # AI-processed text
├── chapter1_final.txt           # Final reviewed version
└── README.md                    # Project documentation



## API Endpoints
- `/scrape` → Scrape book chapter
- `/ai_writer` → AI text processing
- `/human_review` → Manual review
- `/download_final` → Download final text
- `/voice_command` → Control via voice input
- `/rl_feedback` → Reinforcement learning feedback

```

---

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
A short demo video is included in the repository showing the full pipeline execution.



Proof of Completion
CMD showing successful scraping output

CMD showing AI Writer output

CMD showing Human-in-the-Loop output

FastAPI UI showing endpoints

Database versioning success message


