# 📚 Meskerem Primary Worksheet Bank

A modern, cloud-based worksheet management system for teachers at Meskerem Primary School.

## ✨ Features
- 📤 Easy worksheet uploads (PDF, DOC, PPT, Images)
- 📂 Organized by grade and subject
- 👥 Teacher name auto-save
- 📊 Admin dashboard with statistics
- 📱 Fully responsive design
- 🔒 Secure cloud storage with Supabase
- ⚡ Fast global delivery via Vercel

## 🚀 Live Demo
Visit: [https://meskerem-worksheet-bank.vercel.app](https://meskerem-worksheet-bank.vercel.app)

## 🔧 Technology Stack
- **Frontend:** HTML5, CSS3, JavaScript
- **Backend:** Supabase (PostgreSQL)
- **Storage:** Supabase Storage
- **Hosting:** Vercel Edge Network
- **Icons:** Font Awesome 6

## 📋 Setup Instructions

### For Teachers:
1. Visit the website URL
2. Enter your name (saved for next time)
3. Select grade and subject
4. Upload your worksheet
5. Click Upload - Done!

### For Administrators:
1. Click "Admin Panel" at bottom
2. Enter password: `meskerem2026`
3. View statistics or clear all worksheets

## 🗄️ Database Schema
```sql
worksheet (
  id BIGSERIAL PRIMARY KEY,
  teacher_id TEXT,
  grade TEXT,
  subject TEXT,
  file_url TEXT,
  file_name TEXT,
  created_at TIMESTAMPTZ DEFAULT NOW()
)
