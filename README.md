AI Code Review Agent

Built as part of the CipherSchools AI/ML Assignment.

An advanced AI-powered code review system that automatically analyzes GitHub repositories using Abstract Syntax Tree (AST) parsing and Large Language Models (LLMs). The agent generates intelligent review comments with severity levels, confidence scores, and actionable improvement suggestions through an interactive Streamlit dashboard.

Features:

Repository Analysis
Clone public GitHub repositories automatically
Analyze Python source code files
Extract functions and classes using AST parsing
Process repositories in real time
AI-Powered Code Review
Detect potential bugs and code smells
Review code quality and best practices
Generate structured review comments
Provide improvement suggestions

Confidence Scoring:

Every review includes a confidence score (0–100%)
Low-confidence results are separated with a “Verify This” label
Demonstrates responsible AI and uncertainty awareness

Interactive Dashboard:

Clean Streamlit user interface
Real-time progress tracking
Severity-based filtering
Downloadable CSV reports

Tech Stack:

Technology	Purpose
Python	Core programming language
Streamlit	Dashboard UI
Groq LLaMA 3.3 70B	AI code review generation
GitPython	GitHub repository cloning
AST	Source code parsing
Pandas	Data handling
Python-dotenv	Environment variable management

Project Architecture:

GitHub Repository URL
          ↓
Repository Cloning (GitPython)
          ↓
Source Code Parsing (AST)
          ↓
AI Review Engine (Groq API)
          ↓
Confidence Scoring
          ↓
Streamlit Dashboard
          ↓
Downloadable Report

Project Structure:

AI_CODE_REVIEW_AGENT/
│
├── app.py
├── github_clone.py
├── parser.py
├── reviewer.py
├── utils.py
├── requirements.txt
├── .env
└── README.md

Installation Guide:

1. Clone the Repository
git clone <your-github-repo-url>
cd AI_CODE_REVIEW_AGENT
2. Install Dependencies
pip install -r requirements.txt
3. Configure Environment Variables
Create a .env file in the project root:
GROQ_API_KEY=your_api_key_here
4. Run the Application
streamlit run app.py

If Streamlit is not recognized:

python -m streamlit run app.py

Usage:

Launch the Streamlit application
Paste a public GitHub repository URL
Click Analyze Repository
Wait for repository analysis
Review generated AI comments
Filter issues by severity
Download the final CSV report

Key Learning Outcomes:

This project demonstrates practical understanding of:

Agentic AI pipelines
Abstract Syntax Tree parsing
Prompt engineering
Streamlit deployment
Responsible AI principles
Confidence-based reasoning systems
Future Improvements

Planned enhancements include:

Multi-language support
GitHub Pull Request comments
Tree-sitter integration
Repository analytics dashboard
Security vulnerability detection
Code complexity analysis
Docker deployment
Authentication system

Known Limitations:

Currently supports Python repositories only
Large repositories may take longer to analyze
Requires Groq API access
AI responses may occasionally require manual verification.

API key required for live AI review generation.

Author

Srishti Sharma
