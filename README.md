# **AI-Powered Review Aggregator and Sentiment Analyzer**

A multi-agent system that intelligently analyzes YouTube product reviews to generate sentiment-driven summaries and a final verdict. Built using LangGraph, FastAPI, and LLM-based agents, this project demonstrates how autonomous reasoning can be applied to real-world product evaluation at scale.

---

## **Project Highlights**

- **Product Specificity Check**  
  &nbsp;&nbsp;&nbsp;&nbsp;Ensures the query is precise enough for meaningful review retrieval.

- **YouTube Review Scraper**  
  &nbsp;&nbsp;&nbsp;&nbsp;Fetches relevant video IDs based on the user’s product query.

- **Transcript Extraction**  
  &nbsp;&nbsp;&nbsp;&nbsp;Downloads and processes transcripts using the YouTube Transcript API.

- **Relevance Filtering**  
  &nbsp;&nbsp;&nbsp;&nbsp;Uses LLM reasoning to filter out unrelated or off-topic transcripts.

- **Summarization Agent**  
  &nbsp;&nbsp;&nbsp;&nbsp;Generates concise summaries from review content.

- **Verdict Aggregation**  
  &nbsp;&nbsp;&nbsp;&nbsp;Synthesizes all inputs to produce a final recommendation.

---

## **Technologies Used**

- **LangGraph** – Multi-agent orchestration and dynamic flow logic  
- **OpenAI GPT / Groq LLMs** – Filtering, summarization, and reasoning  
- **YouTube Data API + Transcript API** – Review video search and transcript extraction  
- **FastAPI** – Production-ready backend service  
- **Streamlit** – Frontend demo for interactive testing  

---

## **Project Structure**

.
├── agents_modules/
│ ├── product_checker.py
│ ├── youtube_search.py
│ ├── transcript_fetcher.py
│ ├── relevance_filter.py
│ ├── transcript_summarizer.py
│ └── verdict_aggregator.py
├── graph.py 
├── main.py
├── app.py
├── ui.py 
├── requirements.txt
├── .env 
└── README.md


---

## **Getting Started**

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/review-aggregator.git
   cd review-aggregator

2. **Create a Virtual Environment**
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

3. **Install Dependencies**
pip install -r requirements.txt

4. **Set Environment Variables**
Create a .env file in the root directory:

OPENAI_API_KEY=your-openai-key
GROQ_API_KEY=your-groq-api-key

5. **Run the CLI Application**
python main.py

6. **Run Streamlit App**
streamlit run ui.py

7. **Run FastAPI Server**
uvicorn app:app --reload

# **Contributors**
**Mujtaba Junaid**
**Rayan Farhan**
**Anas Soharwardy**


# **Purpose**
What started as an exploration into multi-agent orchestration became a working solution that aggregates public opinion at scale. 
The project showcases how structured LLM workflows can transform raw content (like YouTube reviews) into actionable insights.
A small step toward agentic AI solving real-world problems.

