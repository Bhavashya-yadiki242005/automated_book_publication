Automated Book Publication Project

Overview
This project automates the process of scraping book chapters from an online source, refining the text using AI, enabling human review, and saving different versions of the processed text.
It is built using Python, Playwright, FastAPI, and ChromaDB.

 Features
 Scraping: Extract book content and save text with a screenshot.

 AI Writer: Perform basic AI-powered text transformation.

 Human-in-the-Loop: Allows manual editing of AI-generated text.

 FastAPI UI: Web interface to trigger each process step.

 Database Versioning: Store and retrieve different text versions.
 Project Structure
 automated_book_publication/
│
├── scrape_and_screenshot.py   # Scrapes chapter and takes screenshot
├── ai_writer_reviewer.py      # AI text processing
├── human_feedback_loop.py     # Human review step
├── agentic_api.py             # FastAPI routes
├── db_versioning.py           # Database version control
├── chapter1.txt               # Scraped text
├── chapter1_spun.txt          # AI-processed text
├── chapter1_final.txt         # Final reviewed version
└── README.md                  # Project documentation
How to Run the Project
Create virtual environment (first time only):
bash
python -m venv venv
Activate environment:
bash
venv\Scripts\activate
Install required dependencies:
bash
pip install -r requirements.txt
Run the FastAPI server:
bash
uvicorn agentic_api:app --reload
Open the browser:
Navigate to http://127.0.0.1:8000/docs to access the API UI.

Proof of Completion
Screenshots provided include:

Successful scraping output (CMD)

AI Writer output (CMD)

Human-in-the-Loop output (CMD)

FastAPI UI showing endpoints

Database versioning success message
