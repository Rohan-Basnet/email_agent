# 📧 AI Email Agent

An AI-powered Gmail assistant built using **Google Agent Development Kit (Google ADK)** and the **Groq API**. The agent reads Gmail messages and generates intelligent, context-aware replies on behalf of the user using the Gmail API and OAuth 2.0 authentication.

---

# 🚀 Features

* 🤖 AI-generated email replies
* 📩 Gmail API integration
* 🔐 OAuth 2.0 authentication
* ⚡ Fast inference using Groq LLM
* 🧠 Built with Google ADK
* 🔒 Secure API key management with `.env`
* 📬 Intelligent response generation

---

# 🛠️ Tech Stack

* Python
* Google ADK (Agent Development Kit)
* Groq API
* Gmail API
* Google OAuth 2.0
* Google API Python Client
* python-dotenv

---

# 📁 Project Structure

```text
gmail_agent/
│
├── email_agent/
│   ├── __init__.py
│   ├── agent.py
│   ├── prompt.py
│   └──tools.py  
│
├── .env.example
├── .gitignore
├── requirements.txt
├── README.md
│
├── credentials.json      # Not included in GitHub
└── token.json            # Generated after authentication
```

---

# ⚙️ Installation

### Clone the repository

```bash
git clone https://github.com/Rohan-Basnet/gmail_agent.git
cd gmail_agent
```

### Create a virtual environment

#### macOS/Linux

```bash
python3 -m venv .venv
source .venv/bin/activate
```

#### Windows

```bash
python -m venv .venv
.venv\Scripts\activate
```

### Install dependencies

```bash
pip install -r requirements.txt
```

---

# 🔑 Environment Variables

Create a `.env` file in the project root.

Example:

```env
GROQ_API_KEY=your_groq_api_key
GOOGLE_API_KEY=your_google_api_key
```

---

# 🔐 Gmail API Setup

1. Create a project in Google Cloud Console.
2. Enable the Gmail API.
3. Configure the OAuth Consent Screen.
4. Create OAuth Client Credentials.
5. Download the OAuth credentials.
6. Save the downloaded file as:

```text
credentials.json
```

7. Run the application once and complete the Google authentication flow.

A `token.json` file will be generated automatically after successful authentication.

> **Do not upload `.env`, `credentials.json`, or `token.json` to GitHub.**

---

# ▶️ Running the Agent

Start the Google ADK web interface:

```bash
adk web
```

Or run the agent directly:

```bash
adk run gmail_agent
```

---

# 📌 Workflow

1. Authenticate with your Google account.
2. Gmail API retrieves the email.
3. The email content is processed by the Groq LLM.
4. The AI generates a context-aware reply.
5. The response is returned to the user for review or sending.

---

# 📦 Main Dependencies

* google-adk
* groq
* google-api-python-client
* google-auth
* google-auth-oauthlib
* google-auth-httplib2
* python-dotenv

---

# 🔒 Security

The following files are excluded from version control:

```text
.env
credentials.json
token.json
.venv/
__pycache__/
```

---

# 🚀 Future Enhancements

* ✨ Email summarisation
* 🌍 Multi-language replies
* 📝 Tone customization (Formal, Friendly, Professional)
* 📅 Google Calendar integration
* 📎 Attachment analysis
* ⭐ Priority email detection
* 💬 Conversation memory
* 📊 Email analytics dashboard

---

# 👨‍💻 Author

**Rohan Basnet**

GitHub: https://github.com/Rohan-Basnet

---

# ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub.
