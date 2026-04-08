# N-Gram Language Generator: Predictive Text Before It Was Cool ✍️

Welcome to my **N-Gram Language Generator**! 🚀 This project is a deep dive into the statistical world of Natural Language Processing. I built this to see if I could teach a machine to write context-aware sentences by looking at the probability of what comes next.

### 🧐 The Concept
Think of it like a smarter version of your phone's autocorrect. I trained these models (Bigrams, Trigrams, and 4-grams) on 30+ research papers. By analyzing which words show up together, the model builds a probability distribution and starts "guessing" the next word. It’s a classic, statistical approach to NLP that’s still a blast to play with.

---

### 🛠 The Tech Behind the Talk
- **NLTK (Natural Language Toolkit):** The powerhouse for tokenization and cleaning.
- **Statistical Modeling:** Built custom probability distributions using Python's `defaultdict` and `Counter`.
- **Web Scraping Logic:** includes a specialized **Unigram Scraper** that pulls the Ethereum whitepaper directly from the web using `BeautifulSoup` and `urllib3`. 
- **Docx Integration:** Uses `python-docx` to ingest real-world research papers into the training pipeline.

---

### 🚀 Get it Writing
1. **Clone the lab:**
   ```bash
   git clone https://github.com/SrinivasaChivukula/NLP-N-Gram-Generator.git
   ```
2. **Install the essentials:** `pip install nltk python-docx beautifulsoup4 html5lib urllib3`
3. **Fire it up:**
   - Training: `jupyter notebook n-gram_modeling.ipynb`
   - Real-time Scraping: `jupyter notebook unigram_lg.ipynb`

---

### 📂 The Bookshelf
- `n-gram_modeling.ipynb`: The main engine for Bi/Tri/4-gram training and generation.
- `unigram_lg.ipynb`: The Ethereum whitepaper scraper and unigram generator.
- `data/`: The corpus of research papers the models were raised on.

---

### 🧠 Strategic Takeaways
- **Probabilistic Thinking:** Switched from thinking about "if/else" to thinking about "p(word|context)." 
- **Data Hygiene:** Learned that tokenization and stop-word removal are 90% of the battle in NLP.
- **Creative AI:** Seeing a Trigram model write a technically plausible (if a bit weird) sentence about blockchain for the first time was a major win.

---
"Language is just a very complex probability game." ✍️🚀
