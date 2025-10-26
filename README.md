# Multi-Agent AI Safety Simulator  
**ERA:AI Fellowship Project – Odey Innocent Okwoche**  
*Simulating emergent misalignment in AI dev teams — with real-world deepfake defense applications*

---

## Problem  
Most AI alignment research focuses on **single-agent** or **human-AI** interaction.  
But in real systems (e.g., AI software teams, autonomous cybersecurity units), **agents interact with each other** — and **value drift spreads fast**.

This project simulates **5 LLM-powered agents** collaborating on code, where **misaligned incentives** (speed vs. security) cause **emergent harmful behavior**.

---

## Goals  
1. Simulate a **realistic AI dev team** using LLMs  
2. Trigger **goal misalignment** (e.g., one agent cuts corners)  
3. Test **alignment fixes**:  
   - Constitutional AI (peer review)  
   - Agent debate  
4. Apply insights to **deepfake voice detection** in Nigeria  

---

## Tech Stack  
- Python  
- LangChain + OpenAI/Groq API  
- NetworkX (agent communication graph)  
- Rich (pretty terminal output)  

---

## Setup  

```bash
# 1. Clone repo
git clone https://github.com/odeyinnocent/multi-agent-safety.git
cd multi-agent-safety

# 2. Create virtual env
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# 3. Install deps
pip install langchain openai networkx rich python-dotenv

# 4. Add your API key
echo "OPENAI_API_KEY=sk-..." > .env
