# AI Studies & Projects Repository

A personal repository to organize and share my code and studies in Artificial Intelligence (AI). Each topic is isolated in its own subfolder and managed with a separate [Poetry](https://python-poetry.org/) environment.

This repo includes experiments, notes, and practical projects across a wide range of AI tools and frameworks.

## Topics Covered

- **LLMs** – Large Language Models and their use cases
- **SLMs** – Small Language Models for edge and low-resource scenarios  
- **Practical AI Projects** – End-to-end solutions and hands-on implementations
- **AI App Deployment** – How to deploy AI-powered applications
- **LangGraph** – Graph-based orchestration for LLM workflows
- **Langflow** – Visual interface for chaining LLM components
- **RAG** – Retrieval-Augmented Generation implementations
- **LLM Routing** – Dynamic model routing and intelligent switching
- **PydanticAI** – Structured data validation in AI pipelines using Pydantic

## Structure

Each folder contains:
- `pyproject.toml`: Poetry config
- `.venv/`: Local virtual environment (not pushed to GitHub)
- `src/`: Source code and experiments

Example structure:
```
ai_study/
├── llms/
│   ├── pyproject.toml
│   ├── .venv/
│   └── src/
├── rag/
│   ├── pyproject.toml
│   ├── .venv/
│   └── src/
└── langraph/
    ├── pyproject.toml
    ├── .venv/
    └── src/
```

## Getting Started

1. **Clone the repository**
   ```bash
   git clone [repository-url]
   cd ai_study
   ```

2. **Navigate to any topic folder**
   ```bash
   cd llms/  # or any other topic
   ```

3. **Install dependencies with Poetry**
   ```bash
   poetry install
   ```

4. **Activate the environment**
   ```bash
   poetry shell
   ```

## License 
This project incorporates content from **Scoras Academy**, which is licensed under the [Creative Commons Attribution 4.0 International License (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/).

**Attribution:** Original content by Scoras Academy.

## Notes

- Each topic maintains its own isolated environment to avoid dependency conflicts

---

*This is a living repository that grows with my AI learning journey.*