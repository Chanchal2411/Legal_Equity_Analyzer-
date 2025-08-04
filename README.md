# 🧠 Legal Equity Analyzer using IBM Watsonx.ai

This project is part of the **IBM SkillsBuild Internship (AI & Cloud Technologies)** and aims to analyze **legal equity using Tele-Law data** by leveraging **LLM (Large Language Model)** capabilities from **IBM Watsonx.ai**. It uses foundation models to generate natural language explanations of legal concepts such as equity, access, and justice.

## 🚀 Project Overview

Legal equity is the principle of fairness in legal systems. This project demonstrates how an AI model can understand and explain such abstract legal terms by using generative AI from Watsonx.

> **Use Case:** Tele-Law India, where citizens seek free legal advice via digital means. We help understand and generate insights on how equitable these services are.

---

## 📌 Problem Statement

Analyze the principle of **equity in law** using LLMs by:
- Feeding the model legal definitions, examples, and context from Tele-Law data.
- Generating summaries and human-readable insights using IBM foundation models.
- Providing simple explanations of complex legal fairness issues.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| 🧠 IBM Watsonx.ai | Foundation models / LLM |
| 🐍 Python (Jupyter Notebook) | Development |
| ☁️ IBM Cloud | Deployment |
| 🔐 IBM IAM | API Key / Credential Management |
| 📝 Pandas, Requests | Data handling and API access |

---

## 🔧 Installation

1. Create a new project in [IBM Watsonx.ai](https://dataplatform.cloud.ibm.com).
2. Enable **Foundation Model API Access** in your project settings.
3. Install dependencies:
   ```bash
   pip install ibm-watsonx-ai

## 🧩 Usage

```python
from ibm_watsonx_ai.foundation_models import ModelInference
from ibm_watsonx_ai.credentials import Credentials
```

# Step 1: Set credentials
creds = Credentials(api_key="YOUR_API_KEY", url="https://us-south.ml.cloud.ibm.com")

# Step 2: Set project ID
project_id = "YOUR_PROJECT_ID"

# Step 3: Choose model
model_id = "ibm/granite-13b-instruct-v2"  # or ibm/granite-3-3-8b-instruct (recommended)

# Step 4: Initialize ModelInference
inference = ModelInference(model_id=model_id, credentials=creds, project_id=project_id)

# Step 5: Run inference
prompt = "Explain what legal equity means in simple terms."
result = inference.generate_text(prompt=prompt)
print(result)


💡 Sample Prompts
"Explain equity vs equality in law with an Indian example."

"Is free legal aid an equitable service? Justify."

"What is the role of equity in Tele-Law India?"

📈 Example Output
"Equity is the principle of ensuring fairness and justice by considering individual needs or circumstances, especially when strict application of the law may cause harm or inequality..."

✅ Project Status
✅ API Setup Completed

✅ LLM Model Integrated

✅ Prompt Testing Done

🔄 Optional: Deploy via Flask or Streamlit (Future Scope)

⚙️ Setup Instructions
Install IBM Watsonx AI SDK:

bash
Copy
Edit
pip install ibm-watsonx-ai
Create credentials.json or use inline credentials.

Run notebook locally or on IBM Cloud.

📁 File Structure
Copy
Edit
📦 Legal-Equity-Analyzer/
 ┣ 📜 notebook.ipynb
 ┣ 📜 README.md
 ┣ 📜 requirements.txt
🧪 Requirements
txt
Copy
Edit
ibm-watsonx-ai==1.3.32
pandas
requests
You can install them via:

bash
Copy
Edit
pip install -r requirements.txt
👩‍💻 Author
Chanchal Vishwakarma
IBM SkillsBuild Intern | SRM Institute of Science and Technology

📄 License
This project is licensed under the MIT License.

📚 References
IBM Watsonx.ai Documentation
