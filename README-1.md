# AI Resume ATS System

A resume screening system that parses resumes and job descriptions, scores candidate-role fit, and uses an LLM to explain the result and suggest improvements.

## Features
- **Parsing** of resumes and job descriptions into structured data
- **Fit scoring** based on skills, experience, and keyword relevance
- **Contextual scoring**: related skills and transferable experience count, not just exact keyword overlap
- **LLM explanations**: human-readable reasons why a resume matches or doesn't, plus specific suggestions to improve alignment
- **Extensible design** for batch-processing many resumes against one job description

## Tech Stack
Python, NLP, OpenAI API

## Project Status
Work in progress.

## Getting Started
```bash
git clone https://github.com/<your-username>/ai-resume-ats.git
cd ai-resume-ats
python -m venv venv
venv\Scripts\activate        # Windows
# source venv/bin/activate   # Mac/Linux
pip install -r requirements.txt
python main.py
```

Set your OpenAI key:
```bash
set OPENAI_API_KEY=your_key_here        # Windows
# export OPENAI_API_KEY=your_key_here   # Mac/Linux
```

## How It Works
1. Resume and job description are parsed into structured fields (skills, experience, education).
2. A scoring module compares them using keyword and contextual relevance.
3. The LLM generates an explanation and improvement suggestions.

## Roadmap
- [ ] Batch mode for multiple resumes
- [ ] Simple web UI
- [ ] Export results to CSV/PDF

## Author
Rudraksh Charde
