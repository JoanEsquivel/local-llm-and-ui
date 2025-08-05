# Run a model in your computer

## Global dependencies
```
brew install pyenv
pip install virtualenv
```

## Instructions to create a virtual environment
```
pyenv install 3.11
pyenv shell 3.11
python -m venv venv-311
```

## Instructions to run it in Mac OS
1. Install the ollama library
``` brew install ollama ```
2. Start the service
``` brew services start ollama ```
3. Install the model you want
- Look for the model you want to install locally at the website https://ollama.com/search
- How to install it? I want to try "deepseek-r1:8b"
``` ollama run deepseek-r1:8b ```
4. What commands do we have available for use?
    🧭 Basic Commands

    | Command                  | Description                                                                 |
    |--------------------------|-----------------------------------------------------------------------------|
    | `ollama run <model>`     | Runs a chat session with the specified model (e.g., `ollama run llama3`)    |
    | `ollama pull <model>`    | Downloads a model to your machine                                           |
    | `ollama list`            | Lists all models installed locally                                          |
    | `ollama show <model>`    | Shows metadata and configuration for a model                                |
    | `ollama help`            | Lists all available commands                                                |
    | `ollama version`         | Shows the current version of Ollama                                         |
    | `ollama serve`           | Starts the Ollama local server (required for CLI or API access) - 127.0.0.1:11434             |

5. Is there a good UI tool to interact with the model?
- Check this tool: https://github.com/open-webui/open-webui 
- ``` pip install open-webui ```
- Note: you need Python 3.11 for this tool
- ``` open-webui serve ```
- Visit the website: http://localhost:8080/

6. But also, we can interact with the local LLM just by API requests saba
- Let me work with Jupyter for this demo. If yoy need to set up this for cursor please check this [Setup Jupyter in Cursor video](https://www.youtube.com/watch?v=eOSfeBIBzr0)
- Access to your IDE plugins and look for Jupyter
- Let's create a file with the extension .ipynb. For instance my test.ipvyn. 