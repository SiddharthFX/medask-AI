<<<<<<< HEAD
# Welcome to MedASK AI

## Project info

## How can I edit this code?

There are several ways of editing your application.

**Use your preferred IDE**

If you want to work locally using your own IDE, you can clone this repo and push changes. The only requirement is having Node.js & npm installed - [install with nvm](https://github.com/nvm-sh/nvm#installing-and-updating)

Follow these steps:

```sh
# Step 1: Clone the repository using the project's Git URL.
git clone <YOUR_GIT_URL>

# Step 2: Navigate to the project directory.
cd <YOUR_PROJECT_NAME>

# Step 3: Install the necessary dependencies.
npm i

# Step 4: Start the development server with auto-reloading and an instant preview.
npm run dev
```

**Edit a file directly in GitHub**

- Navigate to the desired file(s).
- Click the "Edit" button (pencil icon) at the top right of the file view.
- Make your changes and commit the changes.

**Use GitHub Codespaces**

- Navigate to the main page of your repository.
- Click on the "Code" button (green button) near the top right.
- Select the "Codespaces" tab.
- Click on "New codespace" to launch a new Codespace environment.
- Edit files directly within the Codespace and commit and push your changes once you're done.

## What technologies are used for this project?

This project is built with:

- Vite
- TypeScript
- React
- shadcn-ui
- Tailwind CSS

### Local Development

To get a local copy up and running follow these simple steps.

- Clone the repo
- Navigate to the root directory in your terminal
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

>>>>>>> db1a8ce (Sanitize repo: add .env.example files, update .gitignore to exclude secrets, and prep for public push)
