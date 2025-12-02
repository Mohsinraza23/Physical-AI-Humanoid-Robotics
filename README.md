# Physical-AI-Humanoid-Robotics

# 🚀 Spec-Kit Plus + Claude Code Router + Gemini  
## **Physical AI & Humanoid Robotics — Essentials (AI-Native Textbook Workflow)**  
**Author:** *Mohsin Raza*  
**Role:** Full-Stack Developer • AI Engineer • PIAIC Student  
**LinkedIn:** https://www.linkedin.com/in/mohsin-raza-a514392b6/

---

# 🌟 QUICK START — INSTALLATION (Windows / PowerShell)

### ✅ **1 — Install Spec-Kit Plus**
```powershell
pip install specifyplus
```

### 🔍 Verify Installation
```powershell
specifyplus --version
```

---

# 📁 CREATE PROJECT FOLDER (Desktop)

```powershell
cd $HOME/Desktop
mkdir my-ai-textbook
cd my-ai-textbook
code .
```

---

# ⚡ Initialize Spec-Kit
```powershell
specifyplus init .
```

### ✔ If using **Claude Paid**  
Just run:
```powershell
claude
```

### ✔ If using **Free Gemini API Key**  
Use Claude Code Router:
```powershell
ccr code
```

---

# 🔥 Claude Code Router + Gemini Setup (FREE)

### **STEP 0 — Confirm Node.js**
```powershell
node --version
```
If not 18+ → download from Node.js official site.

---

### **STEP 1 — Create Google API Key**
Open: https://aistudio.google.com  
Create → API Key  
Copy your key (AIzaSyXXXX etc)

---

### **STEP 2 — Install Global Tools**
```powershell
npm install -g @anthropic-ai/claude-code @musistudio/claude-code-router
```

---

### **STEP 3 — Create Config Folders**
```powershell
mkdir $HOME/.claude-code-router
mkdir $HOME/.claude
```

---

### **STEP 4 — Create config.json**
```powershell
notepad $HOME/.claude-code-router/config.json
```

Paste this JSON **as-is**:

```json
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

---

### **STEP 5 — Add Your API KEY**
```powershell
[System.Environment]::SetEnvironmentVariable('GOOGLE_API_KEY','YOUR_KEY_HERE','User')
```

Check:
```powershell
echo $env:GOOGLE_API_KEY
```

---

### **STEP 6 — Verify**
```powershell
claude --version
ccr version
echo $env:GOOGLE_API_KEY
```

---

### **STEP 7 — Daily Workflow**

**Terminal 1:**
```powershell
ccr start
```

**Terminal 2:**
```powershell
cd your-project
ccr code
```

Test:
```
hi
```

If Claude replies → **Setup is 100% working!** 🚀

---

# 📚 Spec-Kit Plus — OFFICIAL & PERFECT WORKFLOW  

## **STEP 1 — /sp.constitution**
This creates the *DNA* of your project.

Paste this in Claude/Gemini:

```
/sp.constitution

Project Name: Physical AI & Humanoid Robotics — Essentials

Purpose:
Create a short, clean, professional AI-Native textbook based on the Physical AI & Humanoid Robotics course. 
The book must serve as a fast, simple, high-quality learning resource built with a modern Docusaurus UI 
and a fully integrated free-tier RAG chatbot.

Scope:
- 6 short chapters:
  1. Introduction to Physical AI  
  2. Basics of Humanoid Robotics  
  3. ROS 2 Fundamentals  
  4. Digital Twin Simulation (Gazebo + Isaac)  
  5. Vision-Language-Action Systems  
  6. Capstone: Simple AI-Robot Pipeline  
- Clean UI
- Free-tier friendly
- Lightweight embeddings

Core Principles:
- Simplicity  
- Accuracy  
- Minimalism  
- Fast builds  
- Free-tier architecture
- RAG answers ONLY from book text

Key Features:
- Docusaurus textbook  
- RAG chatbot (Qdrant + Neon + FastAPI)  
- Select-text → Ask AI  
- Optional Urdu / Personalize features

Constraints:
- No heavy GPU usage  
- Minimal embeddings  

Success Criteria:
- Build success  
- Accurate chatbot  
- Clean UI  
- Smooth GitHub Pages deployment  

Generate full constitution.
```

---

## **STEP 2 — /sp.specify**
Define the entire textbook.

```
/sp.specify

Feature: textbook-generation

Objective:
Define a complete, unambiguous specification for building the AI-native textbook with RAG chatbot.

Book Structure:
1. Introduction to Physical AI  
2. Basics of Humanoid Robotics  
3. ROS 2 Fundamentals  
4. Digital Twin Simulation (Gazebo + Isaac)  
5. Vision-Language-Action Systems  
6. Capstone  

Technical Requirements:
- Docusaurus  
- Auto sidebar  
- RAG backend (Qdrant + Neon)  
- Free-tier embeddings  

Optional:
- Urdu translation  
- Personalize chapter  

Output:
Full specification.
```

---

## **STEP 3 — /sp.clarify**
Fix unclear points.

```
/sp.clarify
```

---

## **STEP 4 — /sp.plan**  
Generate full implementation plan.

```
/sp.plan textbook-generation
```

---

## **STEP 5 — /sp.tasks**
Generate tasks.md

```
/sp.tasks textbook-generation
```

---

## **STEP 6 — /sp.implement**
Start full code generation.

```
/sp.implement textbook-generation
```

---

# 🧨 FINAL DEPLOYMENT PROMPT (Phase 8)

Paste:

```
Yes, proceed to Phase 8.

Prepare full production deployment for frontend + backend:
- Docusaurus build + GitHub Pages workflow
- Backend deployment (Railway/Render)
- Environment variables
- Health checks
- Launch checklist

Begin Phase 1 after completion.
```

---

# 🏆 RESULT  
✔ Full AI-Native textbook  
✔ 6 chapters auto-generated  
✔ Qdrant + Neon RAG chatbot  
✔ Docusaurus clean UI  
✔ Free-tier optimized  
✔ Claude / Gemini fully connected  
✔ All prompts included  
✔ GitHub-ready README  

---

# ❤️ Created By  
### **Mohsin Raza**  
Full-Stack Developer • AI Engineer • PIAIC Student  
🔥 Passionate about AI, Robotics, and Modern Web  
📌 Karachi, Pakistan


