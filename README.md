# Semantic Book Recommender

A semantic book recommendation system built with LLMs that suggests books
based on meaning and context rather than just keywords.

*Based on freeCodeCamp — Build a Semantic Book Recommender with LLMs*

## Features

- 🔍 **Semantic Search** — vector-based search to find books by meaning, not just keywords (e.g. "a book about a person seeking revenge")
- 🗂️ **Text Classification** — classifies books as fiction or non-fiction using zero-shot classification
- 💬 **Sentiment Analysis** — extracts emotions from text so users can sort by tone (suspenseful, joyful, sad, etc.)
- 🌐 **Web App** — interactive UI built with Gradio

## Project Structure

| File | Description |
|------|-------------|
| `data-exploration.ipynb` | Text data cleaning |
| `vector-search.ipynb` | Semantic search & vector database |
| `text-classification.ipynb` | Zero-shot text classification |
| `sentiment-analysis.ipynb` | Sentiment & emotion analysis |
| `gradio-dashboard.py` | Gradio web application |

## Tech Stack

- Python 3.11
- OpenAI
- Hugging Face
- LangChain
- ChromaDB
- Gradio
- KaggleHub
- Pandas

## Getting Started

### Prerequisites

- Python 3.11
- An [OpenAI API key](https://platform.openai.com/)
- A [Hugging Face API key](https://huggingface.co/settings/tokens)

### Installation

```bash
git clone https://github.com/sophiietran/llm-book-recommender.git
cd book-recommender
pip install -r requirements.txt
```

### Dependencies

| Package | Link |
|---------|------|
| kagglehub | [pypi.org](https://pypi.org/project/kagglehub/) |
| pandas | [pypi.org](https://pypi.org/project/pandas/) |
| matplotlib | [pypi.org](https://pypi.org/project/matplotlib/) |
| seaborn | [pypi.org](https://pypi.org/project/seaborn/) |
| python-dotenv | [pypi.org](https://pypi.org/project/python-dotenv/) |
| langchain-community | [pypi.org](https://pypi.org/project/langchain-community/) |
| langchain-openai | [pypi.org](https://pypi.org/project/langchain-openai/) |
| langchain-chroma | [pypi.org](https://pypi.org/project/langchain-chroma/) |
| transformers | [pypi.org](https://pypi.org/project/transformers/) |
| gradio | [pypi.org](https://pypi.org/project/gradio/) |
| notebook | [pypi.org](https://pypi.org/project/notebook/) |
| ipywidgets | [pypi.org](https://pypi.org/project/ipywidgets/) |

### Dataset

This project uses a book dataset from Kaggle, downloaded via `kagglehub`.
Instructions for setting up Kaggle credentials are included in the tutorial.

### Environment Variables

Create a `.env` file in the root of the project and add the following:

```text
OPENAI_API_KEY=your_openai_key_here
HUGGINGFACE_API_KEY=your_huggingface_key_here
```

> ⚠️ Never commit your `.env` file! Make sure it's listed in your `.gitignore`.

### Running the App

```bash
python3 gradio-dashboard.py
```

Then open your browser and go to the local URL shown in the terminal.
