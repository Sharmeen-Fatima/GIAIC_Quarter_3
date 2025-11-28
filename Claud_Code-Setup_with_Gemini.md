## 🚀 Claude Code + Gemini Full Setup (Windows Guide)

This guide explains how to set up **Claude Code** with **Gemini models** on Windows using
`claude-code` + `claude-code-router`.

---

## ✅ Step 0 — Check Node.js Installation

Open **PowerShell** and run:

```
node --version
```

If your version is **18 or higher**, continue.
If not, install Node.js from:

👉 nodejs.org

---

## ✅ Step 1 — Get Your Google API Key

1. Open: [https://aistudio.google.com](https://aistudio.google.com)
2. Click **"Get API Key"**
3. Click **"Create API Key"**
4. Copy the key (example: `AIzaSy……`)

---

## ✅ Step 2 — Install Required Tools

Open **PowerShell (Run as Administrator)** and run:

```
npm install -g @anthropic-ai/claude-code @musistudio/claude-code-router
```

---

## ✅ Step 3 — Create Configuration Folders

Open **normal PowerShell**:

```
mkdir $HOME/.claude-code-router
mkdir $HOME/.claude
```

---

## ✅ Step 4 — Create config.json (Windows Method)

Windows doesn’t support `cat << EOF`, so use Notepad.

Run:

```
notepad $HOME/.claude-code-router/config.json
```

Notepad will open → Paste the following **exact** JSON:

```
{
  "LOG": true,
  "LOG_LEVEL": "info",
  "HOST": "127.0.0.1",
  "PORT": 3456,
  "API_TIMEOUT_MS": 600000,
  "Providers": [
    {
      "name": "gemini",
      "api_base_url": "https://generativelanguage.googleapis.com/v1beta/models/",
      "api_key": "$GOOGLE_API_KEY",
      "models": [
        "gemini-2.5-flash",
        "gemini-2.0-flash"
      ],
      "transformer": {
        "use": ["gemini"]
      }
    }
  ],
  "Router": {
    "default": "gemini,gemini-2.5-flash",
    "background": "gemini,gemini-2.5-flash",
    "think": "gemini,gemini-2.5-flash",
    "longContext": "gemini,gemini-2.5-flash",
    "longContextThreshold": 60000
  }
}
```

Save and close Notepad.

---

## ✅ Step 5 — Set Your Google API Key (Windows)

Open **PowerShell (Run as Administrator)** and run:

```
[System.Environment]::SetEnvironmentVariable('GOOGLE_API_KEY', 'YOUR_KEY_HERE', 'User')
```

Replace `YOUR_KEY_HERE` with your real API key.

Then close PowerShell → open it again.

Check:

```
echo $env:GOOGLE_API_KEY
```

If it shows your key → ✔ Perfect

---

## ✅ Step 6 — Verify Installation

Run:

```
claude --version
ccr version
echo $env:GOOGLE_API_KEY
```

If all commands return a result → ✔ Setup is correct.

---

## ✅ Step 7 — How to Use (Daily Workflow)

### **Terminal 1: Start Router**

```
ccr start
```

Wait for:

✔ Service started successfully

### **Terminal 2: Run Claude Code**

```
cd your-project-folder
ccr code
```

OR:

```
eval "$(ccr activate)"
claude
```

---

## 🎉 Verification Test

Run:

```
ccr code
```

Then type:

```
hi
```

If Claude replies →
🎉 **Congratulations! Claude Code + Gemini is working!**

---
***✨ Created by [Sharmeen Fatima](https://github.com/sharmeen-fatima).***

- **📫 Feel free to reach out: **✉️ (Sharmeenfatima67@gmail.com).****
- ***✒ For more information about Agentic Ai and updates Join **[Whatsapp Channel](https://whatsapp.com/channel/0029VbAqY7w002TIRJYUHG3X).*****


***“Learning never stops — stay curious, stay creative!”***


***☺️STAY HERE, STAY CONNECTED✨***

