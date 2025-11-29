# **Installation & Setup (Simplified & Professional)**

In Lesson 1, you learned **what Spec-Kit Plus is** and **why it is used**.
Now you will install the framework, verify your tools, and create your first project.

By the end of this lesson, you will have Spec-Kit Plus installed, your AI tool connected, and a test project ready.

---

## **Prerequisite: Python 3.12+**

Spec-Kit Plus requires **Python version 3.12 or higher**.

### **Check your Python version**

Open your terminal or Command Prompt and run:

```
python --version
```

**If you see:**

* `Python 3.12.x` → ✔ You’re ready
* `Python 3.11.x or lower` → ✘ You must install Python 3.12+

---

## **Step 1: Install Spec-Kit Plus**

Once Python 3.12+ is confirmed, install Spec-Kit Plus:

```
pip install specifyplus
```

Verify the installation:

```
specifyplus --version
```

### **What you just installed**

* **specifyplus** — The Spec-Kit Plus framework (includes slash commands, templates, and project creation tools)

### **Important Note**

Spec-Kit Plus is the framework.
Claude Code or Gemini CLI is your AI tool.
**You need both for the system to work.**

---

## **Step 2: Create Your First Project**

Initialize a new Spec-Kit Plus project:

```
specifyplus init my-research-paper
```

During setup, you will be asked:

```
? Select AI Tool:
  > Claude Code
    Gemini CLI

? Select Terminal:
  > bash
    powershell (Windows only)
```

### **Recommended choices**

* **AI Tool:** Claude Code
* **Terminal:** bash (or powershell if you’re on Windows and not using WSL)

---

