# Basic AI Research Agent

A simple AI-powered research assistant that searches the web and Wikipedia to help you research any topic.

## What it does

- Searches the web using DuckDuckGo
- Looks up information on Wikipedia  
- Saves research results to a file
- Returns structured summaries with sources

## Setup

1. **Install Python packages**
   ```bash
   pip install -r requirements.txt
   ```

2. **Add your OpenAI API key**
   Create a `.env` file and add:
   ```
   OPENAI_API_KEY=your-api-key-here
   ```

3. **Run the program**
   ```bash
   python main.py
   ```

## How to use

When you run the program, it will ask: "What can I help you research?"

Type any question like:
- "What is the population of Japan?"
- "Tell me about climate change"
- "History of the internet"

The AI will search for information and give you a summary with sources.

## Example output

```json
{
  "topic": "Population of Japan",
  "summary": "Japan has a population of about 125 million people as of 2023...",
  "sources": ["https://en.wikipedia.org/wiki/Demographics_of_Japan"],
  "tools_used": ["wikipedia", "search"]
}
```

## Files

- `main.py` - Main program that runs the AI agent
- `tools.py` - Search and save functions
- `requirements.txt` - List of needed Python packages
- `.env` - Your API key (you need to create this)

## Requirements

- Python 3.8+
- OpenAI API key
- Internet connection

That's it! Simple research assistant powered by AI.
