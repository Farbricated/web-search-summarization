# 🚀 Web Search and Summarization 🔍✨

This repository contains the Jupyter Notebook `Web_search_and_Summarization.ipynb`, which performs web searches and summarizes results using SerpAPI and Python.

## 📜 Description
The notebook automates web searching and extracts summarized information from search results. It utilizes APIs and Python libraries for efficient data retrieval and summarization.

## 🛠️ Tools & Libraries Used
- 🔎 **SerpAPI** - For fetching search results
- 🏗 **BeautifulSoup** - For web scraping and parsing HTML
- 🌐 **Requests** - For making HTTP requests
- 🤖 **Google Generative AI** - For summarization
- 🎨 **Gradio** - For creating an interactive web UI

## 📝 Sample Code
```python
from serpapi import GoogleSearch
import requests
from bs4 import BeautifulSoup

def google_search(query):
    params = {"q": query, "api_key": "your_serpapi_key", "num": 5}
    search = GoogleSearch(params)
    return search.get_dict().get("organic_results", [])

# Example Usage
results = google_search("Hugging Face AI")
print(results[:3])  # Display first 3 search results
```

## 📜 License
This project is licensed under the MIT License. 📄
