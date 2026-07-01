<h1 align="center">
📖KnowledgeGPT
</h1>

<div id="top" align="center">

![GitHub](https://img.shields.io/github/license/Osama-AI-DEV-UTech/Knowledge_GPT)
![GitHub Repo stars](https://img.shields.io/github/stars/Osama-AI-DEV-UTech/Knowledge_GPT?style=social)
![GitHub forks](https://img.shields.io/github/forks/Osama-AI-DEV-UTech/Knowledge_GPT?style=social)
[![X (formerly Twitter) Follow](https://img.shields.io/twitter)](https://twitter.com/)

</div>

**Accurate answers and instant citations for your documents.**

Upload your documents and get answers to your questions, with citations from the text.

[Demo]()

## Installation

Follow the instructions below to run the Streamlit server locally.

### Pre-requisites

Make sure you have Python ≥3.10 installed.

### Steps

1. Clone the repository

```bash
git clone https://github.com/Osama-AI-DEV-UTech/Knowledge_GPT.git
cd Knowledge_GPT
```

2. Install dependencies with [Poetry](https://python-poetry.org/) and activate virtual environment

```bash
poetry install
poetry shell
```

3. (Optional) Avoid adding the OpenAI API every time you run the server by adding it to environment variables.
   - Make a copy of `.env.example` named `.env`
   - Add your API key to the `.env` file

> **Note:** Make sure you have a paid OpenAI API key for faster completions and to avoid hitting rate limits.

4. Run the Streamlit server

```bash
cd Knowledge_GPT
streamlit run main.py
```

## Build with Docker

Run the following commands to build and run the Docker image.

```bash
cd Knowledge_GPT
docker build -t Knowledge_GPT .
docker run -p 8501:8501 Knowledge_GPT
```

Open http://localhost:8501 in your browser to access the app.

## Customization

You can increase the max upload file size by changing `maxUploadSize` in `.streamlit/config.toml`.
Currently, the max upload size is 25MB for the hosted version.

## Tech Stack

- User Interface - [Streamlit](https://streamlit.io/)
- LLM Tooling - [Langchain](https://github.com/hwchase17/langchain)

## Roadmap

- Add support for more formats (e.g. webpages, PPTX, etc.)
- Highlight relevant phrases in citations
- Support scanned documents with OCR
- More customization options (e.g. chain type, chunk size, etc.)
- Visual PDF viewer
- Support for Local LLMs

## Contributing

All contributions are welcome!


## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=mmz-001/knowledge_gpt&type=Date)](https://star-history.com/#mmz-001/knowledge_gpt&Date)
