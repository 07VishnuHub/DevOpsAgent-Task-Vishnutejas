# 🤖 DevOps AI Agent
An AI-powered autonomous DevOps agent that monitors your infrastructure, detects anomalies, analyzes logs using GPT-4, remediates issues by restarting containers, and notifies your team.

---

## 🧠 What It Does

✅ Monitors system CPU usage using Prometheus  
✅ Identifies which Docker container is consuming the most CPU  
✅ Fetches real-time logs from that container  
✅ Analyzes logs using OpenAI (GPT-4) to identify root cause  
✅ Automatically restarts the container if the LLM recommends  
✅ Sends detailed alerts via email  
✅ Logs all actions to a file

---

## 🛠 Tech Stack

- Python 3.10
- Prometheus + Node Exporter
- Docker (container monitoring)
- LangChain + OpenAI GPT-4
- SMTP (Gmail-based email alerts)

---

## How to run.

- Clone the repo
- Install the requirements
- Setup .env for OPENAI_API_KEY=sk-..., SMTP_USER=your@gmail.com, SMTP_PASS=your_gmail_app_password, ALERT_EMAIL=recipient@example.com
- Run "python3 main.py"

---

## Sample output in mail
🕒 2025-07-06 12:18:57.473065
📦 Container: cpu_hog_app
📈 CPU: 1033.94%
🧠 LLM Analysis:
🔁 Action Taken: ℹ️ Restart not needed — LLM didn’t suggest.

---

👨‍💻 Author
Vishnu — DevOps Engineer
Linkeidn: https://www.linkedin.com/in/vishnutejas07/
