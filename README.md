# MedaskAI: Your Personal AI Health Companion

MedaskAI is a modern, AI-powered health platform that helps users discover, understand, and manage their health using the power of MongoDB, Google Cloud, and generative AI. MedaskAI is designed for production deployment, providing robust, scalable, and privacy-focused health tools for individuals and organizations.

**Live Demo:** [https://tinyurl.com/medask-ai](https://tinyurl.com/medask-ai)

---

## 🌟 Key Features

- **Natural Remedy Finder:** Search 500+ public natural remedies by ailment, ingredient, or keyword, powered by advanced MongoDB Atlas Search and AI summarization.
- **AI Prescription Reader:** Upload a photo of a prescription and receive an instant, patient-friendly AI summary (Google Vision + Gemini AI).
- **AI Health Chat:** Conversational health assistant for personalized Q&A, remedy suggestions, and health education.
- **Personal Health Journal:** Securely track symptoms, queries, and remedies. Journal entries are stored in MongoDB and can be enriched with AI insights.
- **Extensible Platform:** Built for future modules, including symptom checker, nutrition, wearables integration, and telehealth.

---

## 🏗️ Architecture

```
[ React Frontend ]  <-->  [ Express.js API ]  <-->  [ MongoDB Atlas ]
        |                          |                    |
        |--- Google Gemini AI -----|--- Google Vision --|
        |                          |                    |
    (Google Cloud Run: frontend & backend containers)
```

- **Frontend:** React 18, Vite, TypeScript, Tailwind, shadcn-ui
- **Backend:** Node.js, Express, MongoDB Atlas, Google Gemini AI, Google Vision API
- **Authentication:** Supabase (for journal and user data)
- **Deployment:** Google Cloud Run (frontend and backend as separate services)

---

## 🗂️ Data & AI

- **Public Dataset:** 500+ natural remedies, curated from open-access medical literature.
- **MongoDB Atlas:** Flexible, scalable document database with advanced Atlas Search (compound, fuzzy, wildcard, phrase, and vector-ready).
- **Google Gemini AI:** Summarizes remedies, interprets prescriptions, powers health chat.
- **Google Vision API:** OCR for prescriptions and health documents.
- **Supabase:** Secure user authentication and journal storage.

---

## ⚡️ How It Works

1. **User searches for a remedy, uploads a prescription, or asks a health question.**
2. **Backend runs MongoDB Atlas Search** (text, fuzzy, wildcard, phrase, or vector search) on the relevant collection.
3. **Google Vision API** (if image) extracts text from prescriptions.
4. **Google Gemini AI** generates summaries, explanations, or chat responses.
5. **Frontend displays AI-enriched results** with actionable health information.

---

## 🚀 Production Deployment

### Prerequisites
- Node.js, npm/yarn
- MongoDB Atlas cluster
- Google Cloud account (Gemini & Vision API)
- Supabase project (for authentication & journal)

### Backend
```bash
cd server
npm install
# Add .env with MongoDB URI, Gemini API Key, Vision credentials, Supabase keys
npm start
```

### Frontend
```bash
cd frontend
npm install
# Add .env with API base URL and Supabase keys
npm run dev
```

### Cloud Deployment
- Use provided Dockerfiles and `gcloud` commands to deploy both services to Google Cloud Run.
- All environment variables (API keys, URIs) are securely managed in Cloud Run settings.

---

## 🔒 Security & Privacy

- All sensitive data is encrypted in transit (HTTPS).
- No private health data is shared with third parties.
- User authentication and journal entries are secured with Supabase.
- AI services (Gemini, Vision) are used for on-demand inference and never store user data.

---

## 🧩 Extensibility

- **Modular Backend:** Easily add new endpoints for nutrition, symptom checker, or telehealth.
- **Pluggable Frontend:** Add new pages and components for future features.
- **Vector Search Ready:** Platform supports semantic and similarity-based health search.

---

## 🧑‍💻 Contributing

We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines, or open an issue to discuss your ideas.

---

## 🏆 Hackathon Innovation (Optional Section for Judges)

MedaskAI was built for the MongoDB x Google Cloud Hackathon to showcase:
- Real-world impact with a public health dataset
- Advanced use of MongoDB Atlas Search and vector search
- Seamless integration with Google AI and cloud services
- A production-ready, extensible architecture

---

## 🙏 Acknowledgements

- **MongoDB Atlas** for the intelligent data platform.
- **Google Cloud & Gemini AI** for next-gen AI and cloud infrastructure.
- **Open health data community** for the remedies dataset.

---

**Built with ❤️ for real-world health empowerment and innovation.**

---

