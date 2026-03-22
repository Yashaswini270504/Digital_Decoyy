<img width="800" height="334" alt="image" src="https://github.com/user-attachments/assets/88e23e80-df47-48ca-8c58-059a7efe3412" />🛡️ Adaptive Threat Detection System
AI-powered URL threat analysis that thinks beyond binary

The Problem:
Tools like Google Safe Browsing and VirusTotal tell you safe or unsafe
But real-world threats aren't binary — they're coordinated, evolving, and uncertain.

💡 My Solution
I built a system that goes deeper with 4 original techniques:

|     | Technique           | What it does                                          |
| 1️⃣ | Confidence Scoring  | Returns `78% ± 12%` — not just a yes/no                |
| 2️⃣ | Campaign Clustering | Groups attack variants that share the same origin      |
| 3️⃣ | Lifecycle Modeling  | Labels threats as Emerging → Established → Declining   |
| 4️⃣ | Adaptive Learning   | Gets smarter from user feedback — no retraining needed |

⚡ See It In Action:
```python
analyzer = PatentableURLAnalyzer()
result = analyzer.analyze_url("https://suspect-bank-verify.ru/?code=x1")

# Returns:
# ✅ Threat score:     78% ± 12%
# ✅ Lifecycle stage:  Emerging
# ✅ Mutation risk:    High (82%)
# ✅ Campaign match:   3 related URLs detected
# ✅ Top factors:      Suspicious TLD, encoded params, domain squatting

🚀 Run It Yourself:
pip install -r requirements.txt
python app.py

🧠 Why This Is Hard To Build:
- Most ML models need retraining to improve — mine adapts in real-time
- Campaign detection requires behavioral fingerprinting, not just domain matching
- Confidence intervals require uncertainty quantification on top of the base model

🔧 Built With:
`Python` `Flask` `Groq API` `Custom Adaptive Algorithms` `Docker
