CareerMap — Learning Path Generator (MCP Powered)

Live demo: careermap.streamlit.app

One-liner: Generate personalized learning paths from your goals using YouTube, Google Drive, and Notion — orchestrated via the Model Context Protocol (MCP).

🚀 Overview

CareerMap is a Streamlit-based web application that transforms simple goals (e.g., “Learn Python basics in 3 days”) into structured, trackable learning paths.
It leverages MCP (Model Context Protocol) to integrate with:

🎥 YouTube for curated video lessons

📁 Google Drive for storing docs & resources

📝 Notion for note-taking and organization

✨ Features

🎯 Personalized learning paths from a single goal prompt

🎥 YouTube integration for video resources

📁 Google Drive or 📝 Notion as your workspace

📊 Real-time progress tracking

🖥️ User-friendly Streamlit interface

🔌 MCP-based orchestration for clean, extensible integrations

🛠️ Requirements

Python 3.10+

Google AI Studio API Key

Pipedream
 workflows for:

YouTube (required)

Google Drive or Notion (choose one)

⚙️ Installation & Setup
1. Clone & enter the project
git clone <YOUR_REPO_URL> careermap
cd careermap

2. Create & activate a virtual environment
python3 -m venv .venv
source .venv/bin/activate   # Windows: .venv\Scripts\activate

3. Install dependencies
pip install --upgrade pip
pip install -r requirements.txt

4. Configure environment variables

Set your API key + Pipedream URLs. Either export them directly:

export GOOGLE_AI_STUDIO_API_KEY="your_google_ai_studio_api_key"
export PIPEDREAM_YT_URL="https://xxxxxx.m.pipedream.net"     # YouTube workflow
export PIPEDREAM_DRIVE_URL="https://xxxxxx.m.pipedream.net"  # (or) Drive workflow
export PIPEDREAM_NOTION_URL="https://xxxxxx.m.pipedream.net" # (alternative to Drive)


Or place them in a .env file:

GOOGLE_AI_STUDIO_API_KEY=your_google_ai_studio_api_key
PIPEDREAM_YT_URL=https://xxxxxx.m.pipedream.net
PIPEDREAM_DRIVE_URL=https://xxxxxx.m.pipedream.net
PIPEDREAM_NOTION_URL=https://xxxxxx.m.pipedream.net

▶️ Running the App
streamlit run app.py


The app will be live at http://localhost:8501
.

📂 Project Structure
├── app.py              # Main Streamlit application
├── utils.py            # Utility functions and helpers
├── prompt.py           # Prompt templates for MCP
├── requirements.txt    # Python dependencies
└── README.md           # Project documentation

💡 Usage

Open the app in your browser.

Enter your Google AI Studio API key and Pipedream URLs in the sidebar.

Select your preferred secondary tool (Drive or Notion).

Type your goal (e.g., “Learn SQL in 7 days”).

Click Generate Learning Path to receive a day-wise plan with videos, docs, and notes.


Contributions are welcome!

Fork the repo

Create a feature branch

Commit changes

Open a Pull Request
