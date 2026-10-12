# my-agent-demo

## Overview

`my-agent-demo` is a sample project showcasing a documentation agent built with OpenAI's GPT models. The agent assists in creating, updating, and maintaining project documentation such as README files, API references, and contribution guides. It demonstrates how to automate documentation workflows using language models and integrates with a GitHub repository.

## Installation

### Prerequisites

- Python 3.9 or higher
- Git
- An OpenAI API key (optional, if you plan to use the agent's LLM capabilities)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/my-agent-demo.git
   cd my-agent-demo
   ```
2. **Create a virtual environment** (recommended)
   ```bash
   python -m venv .venv
   source .venv/bin/activate   # On Windows use `.venv\Scripts\activate`
   ```
3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
4. **Set up environment variables** (if required)
   ```bash
   export OPENAI_API_KEY=your_openai_key_here
   ```

## Usage

The documentation agent can be run from the command line. Below are a few common commands:

```bash
# Start the documentation assistant
python agent.py
```

### Example: Updating the README

The agent can automatically update the README with new sections:

```python
from doc_agent import DocumentationAgent

agent = DocumentationAgent()
agent.update_readme(section="Installation", content="...your content...")
```

### Example: Generating API Docs

```bash
python generate_api_docs.py
```

## Contribution Guidelines

We welcome contributions! Please follow these steps:

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Make your changes** and ensure the code passes linting and tests.
4. **Commit your changes** with a clear commit message.
5. **Push to your fork**
   ```bash
   git push origin feature/your-feature-name
   ```
6. **Open a Pull Request** against the `main` branch of the original repository.

### Code Style

- Follow PEP 8 guidelines.
- Use type hints where appropriate.
- Run `black` and `flake8` before committing.

### Reporting Issues

If you encounter any bugs or have suggestions, please open an issue on the GitHub repository with a clear description and steps to reproduce.

---

*This README was generated and maintained by the documentation agent.*