# Crew to Tailor Job Applications

This project uses the [CrewAI](https://docs.crewai.com/) framework to automate and enhance the process of tailoring job applications using AI agents. The application extracts information from resumes (PDFs) and matches it with job descriptions to generate personalized applications.

## 🧠 Project Overview

The project orchestrates a team of AI agents, each with a distinct role, to:
- Analyze job descriptions.
- Parse and summarize resumes.
- Generate tailored cover letters or application statements.

## 📁 Project Structure

- `Crew to Tailor Job Applications.ipynb`: The main Jupyter Notebook containing the agent setup, logic flow, and example executions.
- `utils.py`: Utility functions for managing API keys and configuration.
- `ltm_sqlite_storage`: Custom long-term memory storage class for agents (via SQLite).
- Other dependencies handled via Python packages.

## 🚀 Getting Started

### Prerequisites

Ensure you have the following installed:
- Python 3.8+
- [OpenAI API Key](https://platform.openai.com/)
- [Serper API Key](https://serper.dev/)
- `crewai`, `pdfplumber`, and other standard packages.

You can install the required libraries using:

```bash
pip install -r requirements.txt
```

_(Note: You may need to create a `requirements.txt` file with the dependencies used in the notebook.)_

### Environment Variables

Store your API keys using environment variables or a `.env` file:

```bash
export OPENAI_API_KEY=your_openai_key
export SERPER_API_KEY=your_serper_key
```

### Running the Notebook

Open the notebook and run all cells:

```bash
jupyter notebook "Crew to Tailor Job Applications.ipynb"
```

## 🧩 Features

- Modular AI agent-based architecture.
- Resume parsing using `pdfplumber`.
- Long-term memory storage with SQLite for persistent context.
- Easy integration with job boards or application platforms.

## 📌 To Do

- [ ] Add UI for uploading resumes and job descriptions.
- [ ] Expand agent memory capabilities.
- [ ] Deploy as a web app or API service.

## 📄 License

This project is open-source and free to use under the MIT License.

## 🙌 Acknowledgments

- [CrewAI](https://crewai.com)
- OpenAI for LLM APIs
- `pdfplumber` for PDF parsing
