# AI-Agent
AI-Powered App Review Trend Analyzer

An end-to-end Python-based AI agent that scrapes Google Play Store reviews, extracts user issues and feature requests, consolidates similar topics, and analyzes emerging trends using Generative AI and data analytics.

This project is designed to help product teams, analysts, and developers understand real user pain points and improvement opportunities from large volumes of app reviews.

🚀 Features

🔍 Automated Review Scraping from Google Play Store

🧠 AI-based Topic Extraction from unstructured user reviews

🧩 Topic Consolidation to remove duplicates and merge similar issues

📈 Trend Analysis to identify frequently occurring problems & requests

⚙️ Configurable Seed Topics for better domain alignment

🧪 Modular & scalable pipeline design

🗂️ Project Structure
├── main.py                  # Entry point – runs the complete pipeline
├── scraper.py               # Scrapes app reviews from Google Play Store
├── topic_extractor.py       # Uses AI to extract issues/topics from reviews
├── topic_consolidator.py    # Merges similar topics into unified categories
├── trend_analyzer.py        # Analyzes topic frequency and trends
├── seed_topics.json         # Predefined issue & feature seed topics
├── requirements.txt         # Python dependencies
├── .env                     # Environment variables (API keys)
├── .gitignore               # Git ignored files

🧠 How It Works (Pipeline)

Scraping – Fetches recent app reviews using google-play-scraper

Extraction – AI model identifies key complaints, bugs, and requests

Consolidation – Similar issues are grouped (e.g., late delivery + delivery delay)

Trend Analysis – Calculates frequency & highlights dominant themes

🔧 Setup & Installation
1️⃣ Clone the repository
git clone https://github.com/your-username/app-review-trend-analyzer.git
cd app-review-trend-analyzer

2️⃣ Create virtual environment
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate

3️⃣ Install dependencies
pip install -r requirements.txt

🔐 Environment Variables

Create a .env file in the root directory:

GOOGLE_API_KEY=your_google_generative_ai_key


⚠️ Never commit .env files to GitHub.

▶️ Run the Project
python main.py


This will:

Scrape reviews

Extract and consolidate topics

Generate trend insights

📦 Dependencies

google-play-scraper

google-generativeai

pandas, numpy

pydantic

tqdm

python-dotenv

(Full list in requirements.txt)

📊 Example Use Cases

📱 Mobile app product improvement

🧪 UX issue identification

📈 Trend monitoring for releases

🤖 AI-driven customer feedback analysis

🛡️ Best Practices Followed

Modular architecture

Clean separation of concerns

Config-driven topic modeling

Scalable for large datasets

Git-safe configuration handling

📌 Future Enhancements

Dashboard visualization (Streamlit / Power BI)

Multi-language review support

Sentiment scoring per topic

Time-based trend comparison

Export insights to CSV / DB
