# NLP N-Gram Language Generator 🤖

Hey! This project is a dive into the world of **Statistical Natural Language Processing**. It's all about teaching a machine to "speak" by analyzing the relationships between words in a corpus. Basically, it looks at a bunch of text and says, "If I see 'Blockchain is', what's the next word likely to be?"

## 🧐 What's going on here?
This is a probability-based sentence generator. It uses a technique called **N-grams** to predict the next word in a sequence based on the `n-1` previous words. I've tested it with:
- **Bigrams (n=2):** Looking at the previous 1 word.
- **Trigrams (n=3):** Looking at the previous 2 words.
- **4-grams (n=4):** Looking at the previous 3 words for even better context.

The engine digests a set of blockchain research papers and learns how to mimic the academic "tone" of those documents.

---

## 🛠 Tech Stack & Dependencies
To get this NLP engine running, you'll need:

### Software
- **Python 3.9+**
- **Jupyter Notebook/Lab** (to run the `.ipynb` files)

### Python Libraries
Install them all with:
```bash
pip install nltk python-docx beautifulsoup4 html5lib urllib3
```
*Why these?*
- `nltk`: The heavy lifter for tokenization and N-gram utilities.
- `python-docx`: To extract text from Word documents (`.docx`).
- `beautifulsoup4` & `urllib3`: Used in the unigram generator to scrape the Ethereum whitepaper.

---

## 🚀 How to Run
1. **Clone the Repo:**
   ```bash
   git clone https://github.com/SrinivasaChivukula/NLP-N-Gram-Generator.git
   cd NLP-N-Gram-Generator
   ```
2. **Setup Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
3. **Launch the Notebook:**
   ```bash
   jupyter notebook main_notebook.ipynb
   ```
4. **Execution:** Run the cells to see the N-gram models building probabilities and generating "AI-written" sentences about blockchain technology.

---

## 📂 Project Structure
- `main_notebook.ipynb`: The primary NLP engine (N-gram modeling).
- `data/`: Contains the source text (`blockchain_papers.docx`).
- `archive/`: Older iterations, including a Unigram generator that scrapes live data.
- `requirements.txt`: Everything you need to install.

---

## 🧠 Lessons Learned
- **Text Preprocessing is Key:** I learned that proper tokenization (handling case, punctuation, and non-alpha characters) is 90% of the battle in NLP.
- **Statistical Modeling:** Understanding how prefix-target frequencies translate into probability distributions was a big "aha!" moment.
- **Data Extraction:** Learned how to programmatically handle different source formats like `.docx` and live HTML scraping.

---

## 🔮 Future Roadmap
- **Smoothing Techniques:** Implement Laplace or Kneser-Ney smoothing to handle unseen N-grams.
- **Deep Learning Evolution:** Move from statistical N-grams to an LSTM or Transformer-based model.
- **Multi-Source Training:** Train the model on diverse topics to see how the generated "personality" shifts.

---

## 👨‍💻 Author
**Srinivasa Chivukula**  
*Computer Science Major | AIML, CyberSecurity, and Cloud Technologies*

---
"The best way to predict the future is to generate it, one N-gram at a time." 🚀
