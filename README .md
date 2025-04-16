
# 📧 Cold Email Generator using LLMs (Jupyter Notebook)

This project generates personalized cold emails using a large language model (LLM) and optional job description scraping from company websites. It is designed to run entirely within a Jupyter Notebook — no frontend, no hosting, just fast experimentation.

---

## 🚀 Features

- 🔮 Uses **LLM (Groq with LLaMA 3)** for high-quality email generation
- 🌐 **Optional web scraping** to extract job or company info
- 🧠 **Prompt engineering** to customize email tone and content
- 📁 Runs entirely in **Jupyter Notebook** — no need for frontend or deployment
- 📎 (Optional) Portfolio matching from CSV using vector search (ChromaDB)

---

## 🛠️ Requirements

Install dependencies using pip:

```bash
pip install langchain langchain-community langchain-groq chromadb pandas
```

---

## 📁 File Structure

```
email_generator.ipynb      # Main notebook
my_portfolio.csv           # (Optional) CSV with project links and tech stack
README.md                  # This file
```

---

## 📌 How It Works

1. **Initialize** the LLM (via Groq + LLaMA 3)
2. **(Optional)** Scrape a job or company page using `WebBaseLoader`
3. **(Optional)** Extract job-related info like skills, role, etc.
4. **(Optional)** Match your past work (from CSV) using ChromaDB
5. **Generate a cold email** tailored to the job using a prompt template
6. **Display the result** directly in the notebook

---

## 📄 Example Email Prompt

```
Write a short and persuasive cold email introducing our product to the company. 
Use the context from the job description and include relevant project links.
```

---

## 📎 Optional Portfolio CSV Format

If you're using project matching:

```csv
Techstack,Links
"Python, NLP, LLMs",https://example.com/project1
"React, TypeScript",https://example.com/project2
```

---

## 📌 Notes

- This is a **notebook-only project**. No UI or hosting required.
- API key for Groq is required to run the LLM (keep it private!).
- Add markdown cells to guide your usage and experiments.

---

## 📜 License

MIT License
