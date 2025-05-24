# 🧠 Web Summarizer using Ollama + Local LLM (phi3/llama3)

This Python tool fetches the contents of any public webpage, extracts readable content using BeautifulSoup, and sends it to a locally running LLM (like `phi3:mini` or `llama3.2:1b`) via the [Ollama](https://ollama.com) API to generate a concise markdown summary.

## 🚀 Features

* 🌐 Scrape any public website
* 🧽 Strips away navigation and boilerplate text
* 🧠 Uses local LLM models (via Ollama) for private, fast summaries
* ✍️ Output in clean Markdown format

## 📦 Requirements

* Python 3.7+
* [Ollama](https://ollama.com/download) (running locally)
* A model like `phi3:mini` or `llama3.2:1b` pulled using Ollama
* `requests`
* `beautifulsoup4`

Install dependencies:

```bash
pip install requests beautifulsoup4
```

---

## 💠 Usage

1. **Start Ollama** (if not already running):

```bash
ollama run phi3:mini
```

2. **Run the script**:

```bash
python main.py
```

Change the URL inside `main.py` to summarize any site:

```python
url = "https://example.com"
```


## 📂 Project Structure

```bash
.
├── main.py         # Main script to run the summarization
└── README.md       # Project documentation
```


## 🧪 Example Output

For a website like `https://cnn.com`, the output might look like:

```markdown
### Summary of CNN

CNN is a news website covering global events, politics, entertainment, and more. Current headlines include updates on international conflicts, U.S. political developments, and tech news. Key stories include...
```


## 📜 License

This project is open-sourced under the MIT License.
