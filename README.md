# Analysing-the-Teaching-and-Learning-Environments-through-multi-agent-LLMs
# This project contains multiple example scripts that demonstrate how to use local Large Language Models (LLMs) for various natural language processing and report generation tasks.  
You can **replace the API key, API endpoint, model name, and input data path with your own local model or API to adapt it to your use case.

## 1. Project Structure
(1) code_for_sentiment_analysis.py # Sentiment analysis
(2) code_for_topic_identification.py # Topic identification
(3) code_for_report_generation.py # Report generation & optimization
(4) README.md


## 2. Features

### 2.1 Sentiment Analysis
- **Purpose**: Use an LLM to analyze the sentiment of text data.
- **Input**: Tabular data (CSV/Excel) containing a column with text for analysis.
- **Output**: Sentiment classification into three categories:
  - `negative`
  - `positive`
  - `neutral`
---

### 2.2 Topic Identification
- **Purpose**: Use an LLM to extract topics from text data.
- **Input**: Tabular data (CSV/Excel) with a text column.
- **Output**: Topic phrases or keyword groups summarizing the core content.
- **Notes**: You can adjust the prompt to control topic granularity.

---

### 2.3 Report Generation & Optimization
- **Purpose**: Use a multi-agent LLM setup to generate and refine reports.
- **Input**: Image files (e.g., `.png`, `.jpg`).
- **Process**:
  1. Encode the image and send it to the LLM for initial analysis to generate the first report.
  2. Use an optimization agent to refine structure, clarity, and style, producing the second report.
- **Output**: Two Word documents (`.docx`):
  - Initial analysis report
  - Optimized report  
  Saved in the `reports/` folder.
---

## 3. How to Use
1. Install dependencies:
   ```bash
   pip install requests python-docx
