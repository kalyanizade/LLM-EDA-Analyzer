# 📊 LLM-EDA-Analyzer

> Automated Exploratory Data Analysis powered by Local LLM (TinyLlama via Ollama) + Gradio UI

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)
![Gradio](https://img.shields.io/badge/Gradio-UI-orange)
![Ollama](https://img.shields.io/badge/Ollama-TinyLlama-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

---

## 🚀 Overview

**LLM-EDA-Analyzer** is an intelligent, no-code EDA tool that lets you upload any CSV dataset and instantly get:

- 📋 Automated data summary & statistics
- 🧹 Automatic missing value handling
- 📈 Beautiful visualizations (histograms + correlation heatmap)
- 🤖 AI-generated insights powered by a **local LLM** — no API key needed!

---

## ✨ Features

| Feature           | Description                                                     |
| ----------------- | --------------------------------------------------------------- |
| 📂 CSV Upload     | Drag & drop any CSV dataset                                     |
| 🧹 Auto Cleaning  | Fills missing values (median for numeric, mode for categorical) |
| 📊 Visualizations | Distribution histograms + Correlation heatmap                   |
| 🤖 AI Insights    | Local LLM (TinyLlama) analyzes your data summary                |
| 🌐 Web UI         | Clean Gradio interface, shareable via public link               |
| 🔒 100% Local     | No API keys, no data leaves your machine                        |

---

## 🛠️ Tech Stack

- **Python 3.8+**
- **Gradio** — Web UI
- **Pandas** — Data manipulation
- **Matplotlib + Seaborn** — Visualizations
- **Ollama + TinyLlama** — Local LLM for AI insights

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/LLM-EDA-Analyzer.git
cd LLM-EDA-Analyzer
```

### 2. Install Python Dependencies

```bash
pip install -r requirements.txt
```

### 3. Install Ollama & Pull TinyLlama

Download Ollama from [https://ollama.com](https://ollama.com), then run:

```bash
ollama pull tinyllama
```

### 4. Run the App

```bash
python app.py
```

The app will launch at `http://localhost:7860` and also generate a public shareable link.

---

## 📦 requirements.txt

```
gradio
pandas
matplotlib
seaborn
ollama
```

---

## 📁 Project Structure

```
LLM-EDA-Analyzer/
│
├── app.py                  # Main application file
├── requirements.txt        # Python dependencies
├── README.md               # Project documentation
└── sample_data/
    └── sample.csv          # Example CSV to test the app
```

---

## 🧪 How to Use

1. **Launch** the app with `python app.py`
2. **Open** the Gradio URL in your browser
3. **Upload** any `.csv` file
4. **Click Submit** and wait a few seconds
5. **View** your EDA report, AI insights, and charts!

---

## 📊 Example Output

**EDA Report includes:**

- Row/column count
- Mean, std, min, max for numeric columns
- Unique value counts for categorical columns
- Missing value report per column

**Visualizations include:**

- One histogram per numeric column
- A full correlation heatmap

**AI Insights example:**

> *"The dataset shows a right-skewed distribution in the 'Age' column. High correlation (0.87) exists between 'Income' and 'Spending Score'..."*

---

## 🔧 Switching the LLM Model

To use a different local model, edit `app.py`:

```python
# Default
response = ollama.chat(model="tinyllama", ...)

# Other Ollama models you can use:
# model="mistral"
# model="llama3"
# model="gemma"
```

Just run `ollama pull <model-name>` before switching.

---

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgements

- [Ollama](https://ollama.com) — Local LLM inference
- [Gradio](https://gradio.app) — Simple web UI framework
- [Seaborn](https://seaborn.pydata.org) — Statistical data visualization

---

⭐ **If you find this project useful, please give it a star!**
