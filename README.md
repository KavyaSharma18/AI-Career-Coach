# 🚀 AI Career Coach

A comprehensive full-stack AI-powered career development platform that helps users build resumes, prepare for interviews, generate cover letters, and gain industry insights.

## ✨ Features

### 🎯 Core Features
- **AI Resume Builder** - Create professional resumes with AI-powered suggestions
- **Cover Letter Generator** - Generate personalized cover letters for specific job applications
- **Interview Preparation** - Take industry-specific quizzes
- **Industry Insights Dashboard** - Get real-time industry trends, salary data, and career analytics
- **Performance Tracking** - Monitor your progress with detailed analytics and charts

### 🔐 Authentication & User Management
- Secure authentication with Clerk
- Protected routes and role-based access

### 🤖 AI Integration
- Powered by Google Gemini AI for content generation
- Intelligent resume analysis and optimization
- Personalized career recommendations
- Automated background job processing with Inngest

## 🛠️ Tech Stack

### Frontend
- **Next.js 15** - React framework with App Router
- **Tailwind CSS** - Utility-first CSS framework
- **Shadcn/ui** - Modern UI component library
- **Lucide React** - Beautiful icons
- **React Hook Form** - Form validation and management
- **Recharts** - Data visualization and charts

### Backend & Database
- **Prisma ORM** - Type-safe database operations
- **NeonDB** - Serverless PostgreSQL database
- **Clerk** - Authentication and user management
- **Inngest** - Background job processing and workflows

### AI & APIs
- **Google Gemini AI** - Natural language processing and content generation
- **Zod** - Schema validation
- **React Markdown** - Markdown rendering


**Set up environment variables**
   
   Create a `.env` file in the root directory:
   ```env
   # Database
   DATABASE_URL='your-neon-database-url'
   
   # Clerk Authentication
   NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your-clerk-publishable-key
   CLERK_SECRET_KEY=your-clerk-secret-key
   NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
   NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
   NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
   NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding
   
   # Google Gemini AI
   GEMINI_API_KEY=your-gemini-api-key
   ```

## 🗂️ Project Structure

```
├── app/                    # Next.js App Router pages
│   ├── (auth)/            # Authentication pages
│   ├── (main)/            # Main application pages
│   │   ├── dashboard/     # Industry insights dashboard
│   │   ├── resume/        # Resume builder
│   │   ├── ai-cover-letter/ # Cover letter generator
│   │   ├── interview/     # Interview preparation
│   │   └── onboarding/    # User onboarding flow
│   └── api/               # API routes
├── components/            # Reusable React components
│   └── ui/               # Shadcn/ui components
├── actions/              # Server actions for data operations
├── lib/                  # Utility functions and configurations
├── hooks/                # Custom React hooks
├── data/                 # Static data and constants
├── prisma/               # Database schema and migrations
└── public/               # Static assets
```

## 📊 Database Schema

The application uses the following main models:

- **User** - User profiles and preferences
- **Resume** - User resumes with markdown content
- **CoverLetter** - Generated cover letters
- **Assessment** - Interview quiz results and scores
- **IndustryInsight** - Industry trends and salary data

## 🎨 UI Components

Built with modern, accessible components:
- Dark theme by default
- Responsive design for all devices
- Interactive dashboards and charts
- Form validation and error handling
- Loading states and optimistic updates


Made with ❤️ by Kavya Sharma
