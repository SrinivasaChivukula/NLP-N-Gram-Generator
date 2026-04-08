# N-Gram Language Generator ✍️

This project is a deep dive into the statistical side of Natural Language Processing. I built this to explore how machines can "learn" to write by analyzing word probabilities in Bigrams, Trigrams, and 4-gram models.

### 🧠 How it works
I trained these models on a corpus of 30+ research papers. By tracking which words appear together, the generator can predict the most likely next word in a sequence. It’s a classic probabilistic approach to AI that shows how much context matters in language.

### 🛠 Tech Stack
- **NLTK:** For tokenization and text preprocessing.
- **Python:** Custom probability engines built with `defaultdict` and `Counter`.
- **BeautifulSoup:** includes a scraper to ingest real-time data from the Ethereum whitepaper.
- **python-docx:** For bulk processing of Word research documents.

### 🚀 Get Started
1. `pip install nltk python-docx beautifulsoup4 html5lib urllib3`
2. Launch `n-gram_modeling.ipynb` to train and generate text.

---
"Exploring the math behind the message." ✍️🚀
