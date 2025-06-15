# 🧠 MedASK AI — Your Personal AI Health Companion

**MedASK AI** is a full-stack, AI-powered health platform that helps users understand prescriptions, discover natural remedies, and track their health using cutting-edge technologies like **MongoDB Atlas**, **Google Gemini AI**, and **Google Vision API**.

**🌐 Live App:** [https://tinyurl.com/medask-ai](https://tinyurl.com/medask-ai)

---

## 🌟 Features

- 🔍 **Natural Remedy Finder**  
  Search 500+ public natural remedies by ailment, ingredient, or keyword using **MongoDB Atlas Search**.

- 📷 **AI Prescription Reader**  
  Upload a prescription image and receive a simplified AI-generated summary using **Google Cloud Vision OCR + Gemini AI**.

- 💬 **AI Health Chat**  
  Ask health questions, get remedy suggestions, and receive AI-driven explanations using Gemini Pro.

- 📓 **Personal Health Journal**  
  Log symptoms, moods, medications, and notes. Data is securely stored with **Supabase** and visualized with insightful charts.

- 🔧 **Extensible Platform**  
  Future-ready structure for adding nutrition, wearable integration, symptom checker, or telehealth modules.

---

## ⚙️ Architecture

```
[ React Frontend ]  <-->  [ Node.js/Express Backend ]  <-->  [ MongoDB Atlas ]
        |                          |                          |
        |--- Google Gemini AI -----|--- Google Vision OCR ----|
        |                          |                          |
   (Deployed via Google Cloud Run: Frontend & Backend)
```

- **Frontend:** React 18 + Vite + TailwindCSS + shadcn-ui  
- **Backend:** Node.js + Express + Supabase + MongoDB + Google AI  
- **Authentication:** Supabase Auth  
- **Deployment:** Google Cloud Run (containerized)

---

## 📦 Data & AI Integration

- **📚 Natural Remedies Dataset:** 500+ unique remedies, curated from public medical sources and enriched with metadata + imagery.  
- **🔍 MongoDB Atlas Search:** Compound queries (fuzzy, text, wildcard, phrase) for precise remedy discovery.  
- **🧠 Gemini AI:** Used for prescription explanation, chat, and AI summaries.  
- **👁️ Google Vision API:** Extracts text from uploaded prescription images using OCR.  
- **🔐 Supabase:** Secure user auth and journaling database.

---

## 🚀 How It Works

1. **User uploads prescription / searches a remedy / asks a question**
2. **Google Vision API** extracts text (for image uploads)
3. **Gemini AI** processes and generates human-friendly summaries
4. **MongoDB Atlas Search** queries the natural remedies dataset
5. **Frontend displays** personalized insights, results, or visual reports

---

## 🧪 Local Development

### 📁 Backend
```bash
cd server
npm install
# Create .env with:
# MONGODB_URI, GEMINI_API_KEY, SUPABASE_URL, SUPABASE_SERVICE_KEY, etc.
npm start
```

### 🌐 Frontend
```bash
cd frontend
npm install
# Create .env with:
# VITE_API_URL, VITE_SUPABASE_URL, VITE_SUPABASE_ANON_KEY
npm run dev
```

---

## ☁️ Deployment (Google Cloud Run)

- Containerized frontend and backend using Dockerfiles
- Set env variables securely in Cloud Run
- GitHub → Cloud Run CI/CD setup optional

---

## 🔒 Privacy & Security

- All health data is processed in-memory only; not stored by AI services  
- Supabase secures auth and journaling  
- HTTPS enforced via Cloud Run  
- No third-party tracking or sharing

---

## 🧩 Extensibility

- Modular routes for new AI endpoints  
- Add support for wearable data, symptom prediction, teleconsultation  
- Vector Search Ready (for future semantic queries on remedies)

---

## 💡 Built for MongoDB x Google Cloud Hackathon

**Submission Focus:**
- ✔️ Real-world use case (AI + health)
- ✔️ Public dataset powered by Atlas Search
- ✔️ Gemini AI + Google Vision OCR
- ✔️ Scalable, production-grade deployment

---

## 🙏 Acknowledgements

- **MongoDB Atlas** — blazing fast search and flexible document storage  
- **Google Cloud + Gemini AI** — intelligent inference + OCR  
- **Supabase** — frictionless auth and DB  
- **Open Health Data Community** — for public remedy knowledge


**Built with ❤️ for healthcare clarity, empowerment, and AI innovation.**
