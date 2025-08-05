# Run a model in your computer

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
    | `ollama serve`           | Starts the Ollama local server (required for CLI or API access)             |

