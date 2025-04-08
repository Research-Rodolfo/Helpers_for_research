Here's a concise **README.md** for your script:

---

# Virtual Production Web Search Crawler

## 🧠 Overview

This Python script automates Google search queries related to *virtual production*, *education*, *AI*, and *media studies*, parses the search results, classifies the sources, extracts publication years, and saves everything in a structured CSV file.

---

## 🔧 Requirements

Install dependencies:

```bash
pip install requests beautifulsoup4 pandas
```

---

## 📌 Key Features

- **Query Customization**  
  Uses complex Boolean search terms for targeted scraping.

- **Result Parsing**  
  Extracts:  
  `Title`, `Link`, `Snippet`, `SourceType`, and `Publication Year`.

- **Source Classification**  
  Categorizes domains as:
  `Academic Database`, `Blog`, `News Article`, `Video`, etc.

- **Year Extraction**  
  Extracts year via regex from snippets or date spans.

---

## ⚙️ Usage

Run with:

```bash
python your_script.py
```

Modify the `search_queries` list to change keywords.

---

## 📄 Output

Saves results as a `.csv` file named after the query, e.g.:

```
virtual_production_education_film_studies_skills_competencies_teaching_AI.csv
```

---

## 🚨 Notes

- Be cautious of scraping limits and Google’s ToS.
- Script includes a polite delay (`time.sleep(2)`).

---

## 📐 Formula (Conceptual)

\[
\text{Results} = \bigcup_{i=0}^{n} \text{Parse}(\text{HTML}(\text{GoogleSearch}(q, i)))
\]

Where:
- \( q \) = search query  
- \( i \) = page offset  
- `Parse()` = extract fields  
- `Classify()` + `ExtractYear()` enrich result data  

---

Let me know if you want a version that logs errors or supports Bing/Scholar.# Helpers_for_research
