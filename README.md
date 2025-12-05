# 🌟 Yaadein – Collaborative Memory Platform (Web + Mobile + AI Backend)

Yaadein is a next-generation platform that empowers families to **capture, preserve, organize, and relive memories together**.  
It combines an **AI-powered backend**, a modern **React + TypeScript frontend**, and a **Capacitor mobile app** for iOS and Android.

---

# 🚀 Live App

👉 **Web App:** https://yaadein-web-app-pamc.vercel.app/

## ✨ Features

### 👨‍👩‍👧 Family Collaboration
- Create secure family circles  
- Invite members via codes or links  
- Share and relive memories together  

### 📸 Memory Capture & Upload
- Upload photos, videos, and audio  
- Native camera support  
- Batch uploads with progress indicators  

### 🤖 AI-Powered Intelligence
- Automatic tagging  
- Facial recognition  
- AI captions & memory descriptions  
- Smart grouping & suggestions  

### 🔍 Advanced Search
- Search by person, location, timeline  
- “On This Day” memories  
- Voice search  

### 🎮 Cognitive Wellness Games
- Memory recall  
- Daily challenges  
- Activity feed for engagement  

### 🔒 Privacy & Security
- Supabase RLS  
- Family-only control  
- Offline caching  

### 📱 Mobile App Support
- Native Android/iOS builds with Capacitor  
- Offline-first PWA support  

---

# 🧰 Tech Stack

## 🧠 Backend (AI + API)
- Node.js 18+  
- Express + TypeScript  
- Supabase (Auth, DB, Storage)  
- AI Models (HuggingFace + OpenAI)  
  - 📝 Image captioning → Salesforce BLIP  
  - 🧠 Tag generation → Mistral Instruct  
  - 🗣️ Suggestions → DialoGPT-medium  
- Redis + Bull Queues  
- Sharp for image processing  
- Helmet + JWT + rate-limiting  
- Winston logging  

## 🎨 Frontend (Web + Mobile)
- React 18 + TypeScript  
- Tailwind CSS  
- React Router  
- Lucide Icons  
- Supabase client  
- Vite  
- Capacitor (Android + iOS)  

---

# 🚀 Getting Started

## 📦 Prerequisites
- Node.js 18+  
- Supabase project  
- HuggingFace API key  
- OpenAI API key (optional)  
- Android Studio (for Android builds)  
- Xcode (macOS only, for iOS builds)  

---

# 🔧 Backend Setup

### 1️⃣ Clone Repository
```bash
git clone <repo-url>
cd yaadein-backend
npm install
```

### 2️⃣ Environment Setup
```bash
cp .env.example .env
```

Fill in:
- SUPABASE_URL  
- SUPABASE_SERVICE_KEY  
- HUGGINGFACE_API_KEY  
- OPENAI_API_KEY (optional)  

### 3️⃣ Run Backend
```bash
npm run build:server
npm start
```

Backend runs at:  
👉 http://localhost:3000

---

# 🌐 Frontend Setup

### 1️⃣ Install Dependencies
```bash
npm install
```

### 2️⃣ Start Dev Server
```bash
npm run dev
```

Runs at:  
👉 http://localhost:5173

### 3️⃣ Build for Production
```bash
npm run build
```

### 4️⃣ Preview Production Build
```bash
npm run preview
```

---

# 📱 Mobile App (Capacitor)

## 🤖 Android Setup

### Add Android Platform
```bash
npm run cap:add:android
```

### Build Files
```bash
npm run android:build
```

### Open in Android Studio
```bash
npm run android:open
```

### Run on Device/Emulator
```bash
npm run android:dev
```

---

## 🍎 iOS Setup (macOS only)

### Add iOS Platform
```bash
npm run cap:add:ios
```

### Build
```bash
npm run ios:build
```

### Open in Xcode
```bash
npm run ios:open
```

Use Xcode → Archive → Upload to App Store.

---

# 🚢 Deployment

## 🌍 Deploy Web App (Vercel)
- Build Command: `npm run build`  
- Output Directory: `dist`  
- Add required `VITE_` environment variables  

## 🖥️ Deploy Backend (Render / Railway / Fly.io)
Build:
```bash
npm run build:server
```

Start:
```bash
node dist/index.js
```

---

# 📤 Publish on Google Play Store

### Requirements
- Update version codes  
- Signed AAB file  
- Icons (512×512)  
- Screenshots  
- Feature graphic (1024×500)  
- Privacy policy  

### Play Store Compliance
- API level 33+  
- Content rating  
- Store listing with keywords  
- Data safety form  

---

# 🍏 iOS App Store Submission

- Archive in Xcode  
- Upload via Organizer  
- Provide screenshots, privacy disclosures, metadata  

---

# 🔒 Privacy & Security

- Full Supabase RLS  
- Family-level access control  
- Encrypted storage  
- GDPR-compliant data handling  
- Offline cache security  

---

# 🛣️ Roadmap

- 🔔 Push notifications  
- 👤 Better face recognition clustering  
- 🗺️ Memory map visualization  
- 📅 Shared family events  
- 🧵 Threaded comments  
- 🤖 AI-powered story generation  

---

# 🤝 Contributing

We welcome contributions!  
Submit a PR or open an issue for major features or fixes.

---

# 📄 License

MIT License © Yaadein Team

