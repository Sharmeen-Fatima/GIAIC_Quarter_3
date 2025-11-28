# ⚡ Gemini CLI — Installation, Authentication & First Steps (Windows Guide)

This guide provides a clear, beginner-friendly process to install the **Gemini CLI**, verify the setup, and complete authentication on Windows.

---

## ✅ 1. Prerequisites (Check Before You Begin)

Make sure the following are ready:

### **✔ Node.js 20+**

Required for running Gemini CLI.

Check your version:

```powershell
node --version
```

### **✔ npm (Automatically installed with Node.js)**

Verify npm:

```powershell
npm --version
```

### **✔ Google Account**

Any Gmail / Google account is sufficient.

---

## ❓ If Node.js 20+ Is Not Installed

1. Go to: **[https://nodejs.org](https://nodejs.org)**
2. Download the **LTS (Long Term Support)** version
3. Install it (keep the **npm** checkbox enabled)
4. Restart your computer
5. Run the version check again

---

## 🖥️ 2. Open PowerShell (Windows Terminal)

1. Open the **Start Menu**
2. Type **PowerShell**
3. Select **Windows PowerShell**

---

## 📦 3. Install Gemini CLI

### **Method 1: Global Installation (Recommended)**

This installs Gemini CLI permanently on your system.

```powershell
npm install -g @google/gemini-cli
```

---

## 🔍 4. Verify Installation

After installation completes, confirm everything:

### If installed globally:

```powershell
gemini -v
```

You should see a version number (e.g., **0.4.0** or higher).

---

## 🔐 5. Authentication & First Launch

Authentication happens automatically.
Just launch Gemini CLI:

```powershell
gemini
```

On the first run:

* A browser window will open
* You will sign in with your Google account
* Authentication will complete automatically
* Your terminal will return to ready mode

After this, Gemini CLI is fully configured and ready to use.

---

# 🎉 Setup Complete!

You can now use Gemini CLI to run commands like:

```powershell
gemini ask "Create a file named File1.txt and write 5 benefits of AI."
```

Your Gemini CLI is now installed, authenticated, and ready for everyday work.
