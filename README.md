# 🧠 IBM Granite API Clients

This repository contains multi-language code examples for interacting with IBM Granite's Prompt Lab deployment using your IBM Cloud credentials.  
These clients allow you to send prompts and receive structured responses from IBM’s LLM-based deployment.

---

## 📌 Features

- 🔐 Authenticates using IBM Cloud IAM API key
- 🧾 Sends custom prompts (e.g., summarization, drafting, Q&A)
- 🌍 Works across Python, Java, JavaScript, Scala, and Bash
- 📦 Lightweight, clean, ready for integration

---

## 🌐 Languages Supported

| Language   | File                                | Run Command                              |
|------------|-------------------------------------|-------------------------------------------|
| **Python** | `granite_api_call.py`               | `python granite_api_call.py`              |
| **Java**   | `IBMGraniteAPICall.java`            | `javac IBMGraniteAPICall.java && java IBMGraniteAPICall` |
| **JavaScript** | `graniteApiClient.js`           | `node graniteApiClient.js` (with `xmlhttprequest`) |
| **Scala**  | `GraniteApiClient.scala`            | `scala GraniteApiClient.scala` or use SBT |
| **Shell**  | `ibm_granite_api_call.sh`           | `chmod +x ibm_granite_api_call.sh && ./ibm_granite_api_call.sh` |

---

## 🧪 Sample Prompt

All clients send this kind of payload to Granite’s inference API:

```json
{
  "messages": [
    {
      "content": "Summarize the following abstract: AI is transforming education...",
      "role": "user"
    }
  ]
}
