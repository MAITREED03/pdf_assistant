PDF Assistant
A command-line application that creates an AI-powered assistant for interacting with PDF documents using the Phi framework and Groq's LLM.

Features
📚 PDF document processing and analysis
🔍 Vector-based knowledge base search
💾 Persistent chat history storage
🤖 Powered by Groq's llama-3.3-70b-versatile model
📝 Markdown support in responses
Prerequisites
Python 3.8+
PostgreSQL database
Groq API key

Installation
Clone the repository:
git clone https://github.com/yourusername/pdf-assistant.git
cd pdf-assistant

Install dependencies:
pip install -r requirements.txt

Set up environment variables in .env:
GROQ_API_KEY=your_api_key_here

Configure PostgreSQL database (default settings):
Host: localhost
Port: 5532
Database: ai
User: ai
Password: ai

Usage
Start a new conversation:
python pdf_assistant.py --new

Continue existing conversation:
python pdf_assistant.py

Optional parameters:

--new: Start a new conversation
--user: Specify user ID (default: "user")

pdf_assistant/
├── pdf_assistant.py    # Main application file
├── requirements.txt    # Project dependencies
├── .env               # Environment variables
└── README.md         # Project documentation

Dependencies
phi: Core framework for AI assistants
typer: CLI interface
sentence-transformers: Text embedding
psycopg: PostgreSQL adapter
python-dotenv: Environment management


License

MIT

Contributing
Fork the repository
Create your feature branch
Submit a pull request