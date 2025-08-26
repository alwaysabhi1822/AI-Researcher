# 📄 Research AI Agent

An AI-powered research assistant that helps explore recent publications, extract insights, and generate new LaTeX-based research papers.

## 🚀 Features
- **Search arXiv** for recent research papers
- **Read and extract** text from PDF papers
- **Generate research papers** in LaTeX
- **Render LaTeX to PDF** with Tectonic
- **Streamlit frontend** with chat interface
- **LangGraph orchestration** for tool usage

## ⚡ Tools
- `arxiv_search` → fetch papers from arXiv
- `read_pdf` → extract content from PDF
- `render_latex_pdf` → export generated LaTeX papers to PDF

## 🛠️ Setup

### 1. Clone the repo
```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```
### 2. Install dependencies
```
pip install -r requirements.txt
```

### 3. Configure API keys

Create a .env file in the root directory:
```
GOOGLE_API_KEY=your_api_key_here
```
### 4. Run the app
```
streamlit run frontend.py
```
## 📝 Example Usage
```
Ask: “Summarize recent work on quantum computing.”

The agent:

Searches arXiv

Reads PDFs

Suggests new research ideas

Writes a LaTeX paper and renders a downloadable PDF
```

## 📂 Project Structure
```
research-ai-agent/
│── ai_researcher_2.py
│── arxiv_tool.py
│── read_pdf.py
│── write_pdf.py
│── frontend.py
│── requirements.txt
│── .gitignore
│── README.md
│── output/   # generated PDFs
```


### 📄 **requirements.txt**
```
langchain-core==0.3.0
langgraph==0.0.45
langchain-google-genai==0.1.8
requests
PyPDF2
streamlit
python-dotenv
typing-extensions
```
