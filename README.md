# Customer Call Transcript Analyzer

This project is a Python application that uses the Groq API to analyze customer call transcripts for summarization and sentiment analysis.

## Features

-   Analyzes call transcripts using the blazing-fast Groq API.
-   Provides a 2-3 sentence summary of the conversation.
-   Extracts customer sentiment (Positive, Neutral, or Negative).
-   Saves all analysis results to a `call_analysis.csv` file for logging.
-   Built with a FastAPI endpoint for easy integration.

## How to Run This Project

### Prerequisites

-   Python 3.7+
-   A Groq API Key (get one from [GroqCloud](https://console.groq.com/keys))

### Setup

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/Snehapatil334/groq-call-analyzer.git](https://github.com/Snehapatil334/groq-call-analyzer.git)
    cd groq-call-analyzer
    ```

2.  **Create a virtual environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Set up your environment variables:**
    Create a file named `.env` in the project root and add your Groq API key:
    ```
    GROQ_API_KEY="YOUR_API_KEY_HERE"
    ```

5.  **Run the server:**
    ```bash
    uvicorn app:app --reload
    ```

6.  **Test the endpoint:**
    Open your browser and go to `http://127.0.0.1:8000/docs` to access the interactive API documentation.
