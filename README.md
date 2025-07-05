# Agents Project

A comprehensive Python project for building and experimenting with AI agents using various frameworks and tools.

## 🚀 Features

This project includes support for:
- **Anthropic Claude** - Advanced AI models
- **AutoGen** - Multi-agent conversations and workflows
- **LangChain** - LLM application framework
- **LangGraph** - Stateful, multi-actor applications
- **OpenAI** - GPT models and API integration
- **Gradio** - Web-based UI components
- **Playwright** - Web automation
- **Plotly** - Interactive visualizations
- **And more...** - See dependencies below

## 📋 Prerequisites

- Python 3.12 or higher
- [uv](https://github.com/astral-sh/uv) (recommended) or pip

## 🛠️ Installation

### Option 1: Using uv (Recommended)

1. **Install uv** (if not already installed):
   ```bash
   pip install uv
   ```

2. **Clone and navigate to the project**:
   ```bash
   cd learning_agenticai
   ```

3. **Install dependencies**:
   ```bash
   uv sync
   ```

### Option 2: Using pip

1. **Create a virtual environment**:
   ```bash
   python -m venv .venv
   ```

2. **Activate the virtual environment**:
   - Windows:
     ```bash
     .venv\Scripts\activate
     ```
   - macOS/Linux:
     ```bash
     source .venv/bin/activate
     ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

## 📦 Dependencies

### Core AI/ML Libraries
- `anthropic>=0.49.0` - Anthropic Claude API
- `openai>=1.68.2` - OpenAI GPT models
- `langchain-anthropic>=0.3.10` - LangChain Anthropic integration
- `langchain-openai>=0.3.9` - LangChain OpenAI integration
- `langchain-community>=0.3.20` - LangChain community tools
- `langchain-experimental>=0.3.4` - LangChain experimental features

### Agent Frameworks
- `autogen-agentchat>=0.4.9.2` - AutoGen agent conversations
- `autogen-ext[grpc,mcp,ollama,openai]>=0.4.9.2` - AutoGen extensions
- `openai-agents>=0.0.15` - OpenAI agents
- `langgraph>=0.3.18` - Stateful multi-actor applications
- `langgraph-checkpoint-sqlite>=2.0.6` - LangGraph SQLite checkpoints

### Web & UI
- `gradio>=5.22.0` - Web-based UI components
- `playwright>=1.51.0` - Web automation
- `httpx>=0.28.1` - HTTP client
- `requests>=2.32.3` - HTTP library

### Data Processing & Visualization
- `plotly>=6.0.1` - Interactive visualizations
- `pypdf>=5.4.0` - PDF processing
- `pypdf2>=3.0.1` - PDF processing (legacy)
- `bs4>=0.0.2` - BeautifulSoup for web scraping
- `lxml>=5.3.1` - XML/HTML processing

### Development & Utilities
- `python-dotenv>=1.0.1` - Environment variable management
- `ipywidgets>=8.1.5` - Jupyter widgets
- `psutil>=7.0.0` - System and process utilities
- `semantic-kernel>=1.25.0` - Microsoft Semantic Kernel
- `sendgrid>=6.11.0` - Email services
- `wikipedia>=1.4.0` - Wikipedia API
- `polygon-api-client>=1.14.5` - Financial data API
- `speedtest-cli>=2.1.3` - Internet speed testing

### Development Dependencies
- `ipykernel>=6.29.5` - Jupyter kernel

## 🔧 Usage

### Basic Setup

1. **Set up environment variables** (create a `.env` file):
   ```bash
   # OpenAI
   OPENAI_API_KEY=your_openai_api_key_here
   
   # Anthropic
   ANTHROPIC_API_KEY=your_anthropic_api_key_here
   
   # Other services as needed
   ```

2. **Start experimenting**:
   ```python
   # Example: Using OpenAI
   import openai
   from langchain_openai import ChatOpenAI
   
   # Example: Using Anthropic
   import anthropic
   from langchain_anthropic import ChatAnthropic
   
   # Example: Using AutoGen
   import autogen
   ```

### Project Structure

```
learning_agenticai/
├── pyproject.toml          # Project configuration
├── requirements.txt        # Compiled dependencies
├── uv.lock               # uv lock file
├── .venv/                # Virtual environment
├── .python-version       # Python version specification
└── README.md            # This file
```

## 🎯 Common Commands

### Using uv
```bash
# Install dependencies
uv sync

# Add a new package
uv pip install package_name --sync

# Update dependencies
uv pip compile pyproject.toml -o requirements.txt

# Run a Python script
uv run python your_script.py
```

### Using pip
```bash
# Install from requirements.txt
pip install -r requirements.txt

# Install a new package
pip install package_name

# Update requirements.txt
pip freeze > requirements.txt
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test your changes
5. Submit a pull request

## 📄 License

This project is licensed under the terms specified in the LICENSE file.

## 🆘 Troubleshooting

### Common Issues

1. **Package conflicts**: Try `uv sync` to ensure environment matches `pyproject.toml`
2. **API key errors**: Make sure your `.env` file is properly configured
3. **Version conflicts**: Use `uv pip compile` to resolve dependency conflicts

### Getting Help

- Check the [uv documentation](https://docs.astral.sh/uv/)
- Review the [LangChain documentation](https://python.langchain.com/)
- Explore [AutoGen documentation](https://microsoft.github.io/autogen/)

## 🚀 Next Steps

- Create your first agent script
- Experiment with different AI models
- Build multi-agent workflows
- Develop web interfaces with Gradio
- Explore LangGraph for complex stateful applications

---

**Happy coding with AI agents! 🤖✨** 