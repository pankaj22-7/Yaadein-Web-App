# Yaadein - Collaborative Memory Platform with AI-powered Backend

Yaadein is a platform for families to preserve, organize, and share precious memories. It includes an AI-driven backend for analyzing and tagging photos, facial recognition, and interactive memory games. The platform also features a mobile app for iOS and Android, built with React, TypeScript, and Capacitor.

---

## 🎯 Project Overview

Yaadein is a robust memory management system powered by advanced AI models. The platform allows families to upload photos, videos, and audio recordings, collaborate on organizing and tagging memories, and engage in memory games. The backend handles intelligent photo tagging, facial recognition, and dynamic game sessions, while the frontend (web and mobile) provides a seamless user experience.

---

## 🏗️ Technology Stack

### Backend (Yaadein AI Backend)

- **Runtime**: Node.js 18+ with Express.js
- **Language**: TypeScript for type safety and better development experience
- **AI Models**: Hugging Face Inference API + OpenAI Vision API fallback
  - **Primary**: `Salesforce/blip-image-captioning-large` for image captioning
  - **Secondary**: `microsoft/DialoGPT-medium` for conversational tag suggestions
  - **Facial Recognition**: `microsoft/DialoGPT-medium` for face detection
  - **Tag Generation**: `mistralai/Mistral-7B-Instruct-v0.1` for intelligent tagging
- **Database**: Supabase PostgreSQL with Row Level Security (RLS)
- **File Storage**: Supabase Storage with CDN optimization
- **Image Processing**: Sharp.js for optimization
- **Caching**: Redis for high-performance caching
- **Queue Management**: Bull Queue for background processing
- **Security**: Helmet.js, rate limiting, input validation with Express Validator
- **Monitoring**: Winston logging

### Frontend (Web and Mobile)

- **Frontend**: React 18 + TypeScript + Tailwind CSS
- **Mobile**: Capacitor for native iOS/Android apps
- **Icons**: Lucide React
- **Routing**: React Router
- **Build Tool**: Vite
- **Backend**: Supabase (Auth, Database, Storage)

---

## 🚀 Getting Started

### Prerequisites

- **Backend**: 
  - Node.js 18+
  - Redis server
  - Supabase account and project
  - Hugging Face API key (for AI features)
  - OpenAI API key (optional, for fallback)
  
- **Frontend**: 
  - Node.js 18+ and npm
  - Android Studio (for Android development)
  - Xcode (for iOS development, macOS only)

---

### Backend Installation

1. Clone the backend repository:
   ```bash
   git clone https://github.com/yourusername/yaadein-ai-backend.git
   cd yaadein-ai-backend
