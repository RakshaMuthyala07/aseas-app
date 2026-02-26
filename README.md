# ASEAS — Automated Script Evaluation & Analysis System

Deploy in **2 minutes** and get a shareable link.

---

## 🚀 Deploy to Vercel (Free — Get a live link)

### Step 1 — Upload to GitHub
1. Go to [github.com](https://github.com) → New repository → name it `aseas-app` → Create
2. Upload all these project files (drag and drop the folder)

### Step 2 — Deploy on Vercel
1. Go to [vercel.com](https://vercel.com) → Sign up free with GitHub
2. Click **"Add New Project"** → Import your `aseas-app` repo
3. Framework: **Create React App** (auto-detected)
4. Click **"Environment Variables"** → Add:
   - Key: `ANTHROPIC_API_KEY`
   - Value: `sk-ant-...` (your Anthropic API key from console.anthropic.com)
5. Click **Deploy**

✅ You'll get a link like: `https://aseas-app.vercel.app`

Share that link — anyone who opens it can upload a handwritten script and get it graded instantly.

---

## What the app does
1. **Upload** a photo of a handwritten answer script (JPG/PNG)
2. **Claude Vision OCR** reads the actual handwriting and extracts the text
3. **Set rubric** — subject, total marks, reference answer
4. **AI grades** the answer using RAG + rubric-constrained LLM
5. **Results** — score, grade, question breakdown, strengths, improvements

## Tech Stack
- React (frontend)
- Claude claude-sonnet-4 Vision (real OCR)
- Claude claude-sonnet-4 LLM (rubric-constrained grading)
- Vercel (hosting + serverless API proxy)
