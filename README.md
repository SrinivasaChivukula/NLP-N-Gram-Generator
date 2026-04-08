# NLP N-Gram Language Generator 🤖

Hey! So, I've been geeking out on **Statistical Natural Language Processing** lately, and this project is the result. It’s all about teaching a machine how to "talk" by analyzing how words hang out together in a corpus. Basically, the engine looks at a mountain of text and tries to guess: *"Hey, if I just said 'Blockchain is', what's the next word most likely to be?"*

## 🧐 What's the secret sauce?
This isn't just a random word flinger; it's a probability-based sentence generator. I’m using **N-grams**, a classic NLP technique that predicts the next word in a sequence based on the `n-1` words that came before it. 

I’ve built models for:
- **Bigrams (n=2):** The "quick and dirty" approach—looks back exactly one word.
- **Trigrams (n=3):** Getting a bit smarter—checks the previous two words for better flow.
- **4-grams (n=4):** The high-fidelity mode—looks at 3-word chunks to capture actual academic patterns.

The model "trains" on a bunch of blockchain research papers. The result? Sentences that actually sound like they came from a crypto-enthusiast (even if they occasionally go off the rails).

---

## 🛠 Prerequisites & The Tech Stack
To get this engine running on your rig, you’ll need:

### Software
- **Python 3.9+** (obviously!)
- **Jupyter Notebook/Lab** (to run the `.ipynb` files and see the magic happen)

### The Libraries
You can grab everything with one command:
```bash
pip install nltk python-docx beautifulsoup4 html5lib urllib3
```
*Wait, why do we need all these?*
- **`nltk`**: The goat of NLP. It handles the tokenization and the N-gram heavy lifting.
- **`python-docx`**: Because manually copying text from Word docs is for suckers.
- **`beautifulsoup4` & `urllib3`**: These are used in the unigram generator to scrape the Ethereum whitepaper directly from the web.

---

## 🚀 How to Run
Ready to generate some AI babble? 
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
4. **Ignition:** Just run the cells. You'll see the probability models building in real-time and spitting out generated sentences.

---

## 📂 Project Structure
I’ve revamped the layout to keep it clean:
- `main_notebook.ipynb`: The main NLP engine. This is where the N-gram magic lives.
- `data/`: The "brain" of the model—contains `blockchain_papers.docx`.
- `archive/`: Older experiments, including a Unigram generator that scrapes live data.
- `requirements.txt`: The shopping list of libraries.

---

## 🧠 What I Learned (The hard way)
- **Tokenization is 90% of the job:** You wouldn't believe how much noise is in raw text. Handling case, punctuation, and "trash" characters is what makes or breaks a model.
- **Statistical Fidelity:** There’s a sweet spot between Bigrams (too random) and 4-grams (too rigid). Finding that balance was a huge "aha!" moment.
- **Automated Extraction:** Dealing with `.docx` files and web scraping taught me a lot about data pipelines before the NLP even starts.

---

## 🔮 Future Roadmap
- **Smoothing:** Implement Laplace or Kneser-Ney smoothing to handle those annoying "unseen" word combos.
- **The Neural Leap:** Move from statistical counts to an LSTM or Transformer-based model (GPT-style).
- **Sentiment Layers:** Try to force the model to generate only "positive" or "skeptical" sentences.

---

## 👨‍💻 About the Author
**Srinivasa Chivukula**  
*Computer Science Major | AIML, CyberSecurity, and Cloud Technologies*

---
"The best way to predict the future is to generate it, one N-gram at a time." 🚀
