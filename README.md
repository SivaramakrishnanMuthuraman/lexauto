# ⚖️ LexCopra — Product Liability in Cars | COPRA 2019

> An AI-powered legal research chatbot for **Product Liability in Automobiles** under the **Consumer Protection Act 2019 (COPRA 2019)**, Chapter VI (Sections 82–87).

Analyses your car defect matter by citing **90 judicial precedents** and applicable statutory provisions — strictly from the provided database. No external case law. No self-generated conclusions.

---

## 🚀 Deploy on GitHub Pages

### Step 1 — Create a Repository

1. Go to [github.com](https://github.com) → Click **New repository**
2. Name it (e.g., `copra-chatbot`) → Set to **Public** → Click **Create repository**

### Step 2 — Upload the File

Upload `index.html` (and this `README.md`) to the root of the repository.

**Via GitHub web interface:**
- Open your repository → Click **Add file** → **Upload files** → drag and drop both files → **Commit changes**

**Via Git (terminal):**
```bash
git init
git add index.html README.md
git commit -m "Deploy LexCopra chatbot"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/copra-chatbot.git
git push -u origin main
```

### Step 3 — Enable GitHub Pages

1. Go to your repository → **Settings** → **Pages**
2. Under **Source** → select `Deploy from a branch`
3. Choose `main` branch → `/ (root)` → Click **Save**
4. Wait ~60 seconds. Your site will be live at:

```
https://YOUR_USERNAME.github.io/copra-chatbot
```

---

## 🔑 Activating the AI

The chatbot uses the **Anthropic Claude API**. To enable it:

1. Get your API key at [console.anthropic.com](https://console.anthropic.com)
2. Open the deployed site in your browser
3. In the **left sidebar**, find the **Anthropic API Key** field
4. Paste your key (`sk-ant-…`) and click **Save**

Your API key is stored in your **browser's `localStorage` only** — it is never sent anywhere except directly to Anthropic's servers.

---

## 📋 Features

| Feature | Description |
|---|---|
| **AI Legal Chatbot** | Step-by-step guided analysis — identifies defect type, liable party, timeline, and remedy sought before citing relevant cases |
| **90 Case Laws** | Supreme Court & NCDRC judgments covering 11 defect categories |
| **Case Browser** | Search and filter all 90 cases; click any card for full details including ratio decidendi and judgment link |
| **COPRA Provisions** | Sections 82–87 with full statutory text, definitions, and judicial notes |
| **Strict Source Control** | AI is locked by system prompt to the provided database only — no hallucinated cases, no self-drawn conclusions |
| **Analysis Progress Tracker** | Sidebar tracker showing 4 stages: Defect → Party → Timeline → Remedy |
| **Cited Cases Sidebar** | Cases referenced in the conversation appear live in the chat sidebar |

---

## 📚 Case Categories (90 Total)

| Category | Cases |
|---|---|
| Electronics | 18 |
| Airbag & Safety | 13 |
| Services / Dealer Liability, Warranty Denial & Delay in Repairs | 13 |
| Engine | 12 |
| Brakes | 10 |
| Unfair Trade Practices / Deceptive Sales, Model Year Fraud & Financial Extortion | 10 |
| Misleading Advertisements / Mileage Claims, Brochure Discrepancies & Delivery Delays | 6 |
| Suspension / Tyre Wear & Structural Defects | 3 |
| Structural / Body & Build Defects | 2 |
| EV Architecture / Battery, Fire & Thermal Defects | 2 |
| Electronics / Infotainment & Display System Defects | 1 |

---

## 📁 Project Structure

```
copra-chatbot/
├── index.html      ← Complete single-file application (all data, logic, and UI embedded)
└── README.md       ← This file
```

The entire application — 90 case laws, COPRA provisions, chatbot logic, and UI — is contained in `index.html`. No build step, no server, no external dependencies except Google Fonts and the Anthropic API.

---

## ⚖️ Legal Disclaimer

- This tool is for **educational and research purposes only**
- It does **not constitute legal advice**
- All answers are based **strictly** on the provided case database and COPRA 2019 provisions
- Always consult a **qualified legal professional** for actual legal matters

---

## 📜 Sources

- **Case Laws** — AI Case Analysis Sheet (90 curated judicial precedents)
- **Statutory Provisions** — *Product Liability in Respect of Cars under COPRA 2019* (provided document)
- **Statute** — Consumer Protection Act, 2019, Chapter VI, Sections 82–87

---

*Built for academic and research purposes in Indian consumer law.*
