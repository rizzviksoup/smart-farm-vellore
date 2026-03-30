# 🌾 Smart Farm Management System — Vellore, Tamil Nadu

Live dashboard built with Streamlit. Fetches real weather + soil data from Open-Meteo every 30 minutes.

---

## 🚀 Deploy to Render.com (FREE — step by step)

### Step 1 — Push to GitHub

1. Go to https://github.com and create a free account (if you don't have one)
2. Click **New repository** → name it `smart-farm-vellore` → click **Create repository**
3. On your PC, open a terminal/command prompt in this folder and run:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/smart-farm-vellore.git
git push -u origin main
```

(Replace `YOUR_USERNAME` with your GitHub username)

---

### Step 2 — Deploy on Render.com

1. Go to https://render.com and sign up (free, use your GitHub account)
2. Click **New +** → **Web Service**
3. Click **Connect a repository** → select `smart-farm-vellore`
4. Fill in the form:
   - **Name**: `smart-farm-vellore` (or anything you like)
   - **Region**: Singapore (closest to Vellore)
   - **Branch**: `main`
   - **Runtime**: `Python 3`
   - **Build Command**: `pip install -r requirements.txt`
   - **Start Command**: `streamlit run app.py --server.port $PORT --server.address 0.0.0.0`
5. Under **Instance Type** → select **Free**
6. Click **Create Web Service**

Render will build and deploy. In ~3 minutes your dashboard will be live at:
`https://smart-farm-vellore.onrender.com`

---

## 💻 Run locally (on your own PC)

```bash
pip install -r requirements.txt
streamlit run app.py
```
Opens at http://localhost:8501

---

## 📁 Files

| File | Purpose |
|------|---------|
| `app.py` | Main Streamlit dashboard |
| `requirements.txt` | Python dependencies |

---

## 🔄 Data refresh

- Dashboard caches weather data for **30 minutes** automatically
- Use the **🔄 Refresh data** button in the sidebar to force a fresh fetch
- Open-Meteo API is free, no key needed

---

## 📊 Features

- 7 interactive charts across tabs
- Live weather + soil conditions
- Per-crop irrigation / pesticide / fertilizer / harvest alerts
- Water saving comparison vs traditional farming
- Fertilizer schedule with upcoming events
- Mobile-friendly layout
"# smart-farm-vellore" 
