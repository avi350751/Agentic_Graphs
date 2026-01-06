SIMPLE-LANGGRAPH 🧩
A beginner-friendly LangGraph playground that demonstrates how to build graphs and sequential LLM workflows using typed state, nodes, and edges—all in small, runnable Jupyter notebooks.
This repo is set up as a learning module with 3 progressive notebooks:


- start with a minimal graph,
- build a simple LLM workflow,
- implement prompt chaining as a sequential graph (e.g., title → outline → content → scoring).



What you’ll learn


How LangGraph works (StateGraph, nodes, edges, START/END)
Designing typed state using TypedDict
Building different workflows with ChatOpenAI
Running everything inside notebooks with clean, repeatable setup



Repository Structure
SIMPLE-LANGGRAPH/
├─ 1_test_simple_graph.ipynb         # smallest possible LangGraph example
├─ 2_simple_llm_workflow.ipynb       # basic LLM-in-the-loop graph workflow
├─ 3_prompt_chaining.ipynb           # sequential prompt chaining using state
├─ requirements.txt                  # python dependencies
├─ .env                              # API keys (not recommended to commit)
└─ langenv/                          # local virtual environment (optional)


Quickstart
1) Create & activate a virtual environment
macOS / Linux
python -m venv langenv
source langenv/bin/activate

Windows (PowerShell)
python -m venv langenv
.\langenv\Scripts\Activate.ps1

2) Install dependencies
If you use uv:
uv pip install -r requirements.txt

Or standard pip:
pip install -r requirements.txt

3) Add your API key
Create a .env file in the repo root:
OPENAI_API_KEY=your_key_here


The notebooks use load_dotenv() so your environment variables load automatically.

4) Run the notebooks
Using Jupyter:
jupyter notebook

Or open the folder in VS Code and run cells from the notebook UI.