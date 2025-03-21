
# **Financial Data Extractor**  

Extract financial metrics like revenue and EPS from text using Large Language Models (LLMs).

Application link: https://llm-financial-data-extractor-vraj-dobariya.streamlit.app/
---

## Overview

`llm-financial-data-extractor` leverages the power of Large Language Models (LLMs) to extract financial data from unstructured text, such as news articles or financial reports. Built with `langchain-groq` and the `llama-3.3-70b-versatile` model, it extracts key metrics—actual and expected revenue and earnings per share (EPS)—and outputs them in a structured JSON format. The project includes a Streamlit-based web interface for easy interaction, making it accessible to both developers and non-technical users.

### Features
- Extracts `revenue_actual`, `revenue_expected`, `eps_actual`, and `eps_expected` with units (e.g., million, billion).
- Streamlit UI for inputting text and viewing results in a table.
- Licensed under Apache License 2.0.

---

## Installation

### Prerequisites
- Python 3.8 or higher
- A Groq API key (for LLM access)

### Steps
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/Vraj-Data-Scientist/llm-financial-data-extractor.git
   cd llm-financial-data-extractor

## Install Dependencies:
  ```bash

  pip install -r requirements.txt
  ```

### Dependencies include:
streamlit  
langchain-groq  
dotenv  

## Set Up Environment Variables: Create a .env file in the project root and add your Groq API key:

```text
GROQ_API_KEY=your-api-key-here
```

## Project Structure

- .gitignore: Excludes Python bytecode, build artifacts, environments, and tool caches.
- data_extractor.py: Core extraction logic using langchain-groq and the llama-3.3-70b-versatile LLM.
- app.py: Streamlit frontend for user interaction.
- requirements.txt: Lists project dependencies.
- LICENSE: Apache License 2.0.

## Limitations

- Context Size: Large inputs may fail due to LLM context limits.
- Metric Scope: Currently limited to revenue and EPS.
- API Dependency: Requires a Groq API key and internet access.
