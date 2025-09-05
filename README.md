Sensei — AI Career Coach

Sensei is a full-stack AI-powered career coach built with Next.js, React, and Tailwind CSS.
It helps users build professional resumes, generate cover letters, practice mock interviews, and receive AI-driven feedback to level up their careers.

Table of Contents

Features

Tech Stack

Project Structure

Getting Started

Environment Variables

Usage

Contributing

Future Enhancements

Acknowledgements

License

Features

User Authentication & Onboarding (Clerk)

AI Career Guidance using Gemini AI API

Resume Builder with PDF export

Cover Letter Generator

Mock Interviews with performance tracking

Progress Dashboard & Analytics

Automated Tasks with Inngest

Tech Stack

Frontend: Next.js (React), Tailwind CSS, Shadcn UI

Backend: Next.js API routes, Prisma ORM with NeonDB (PostgreSQL)

Authentication: Clerk

AI Integration: Gemini API

Job Scheduling: Inngest

PDF Generation: PDFKit

Deployment: Vercel

Project Structure
.
├── app/                # Next.js pages and routes
├── components/         # Reusable UI components
├── data/               # Static or seed data
├── hooks/              # Custom React hooks
├── lib/                # Helper functions and utilities
├── prisma/             # Prisma schema & migrations
├── public/             # Static assets (images, icons, etc.)
├── .env                # Environment variables (not committed)
├── package.json        # Dependencies and scripts
└── README.md

Getting Started
1. Clone the Repository
git clone https://github.com/piyush-eon/ai-career-coach.git
cd ai-career-coach

2. Install Dependencies
npm install

3. Set Up Database
npx prisma migrate dev

4. Run the Development Server
npm run dev


Visit http://localhost:3000

Environment Variables

Create a .env file in the root directory and add the following:

DATABASE_URL=<NeonDB/PostgreSQL URL>
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=<Clerk publishable key>
CLERK_SECRET_KEY=<Clerk secret key>

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding

GEMINI_API_KEY=<Gemini AI API key>

Usage

Sign up / Log in with Clerk.

Set up career goals during onboarding.

Build resume → download as PDF.

Generate cover letters tailored to job applications.

Practice mock interviews with AI feedback.

Track progress in the analytics dashboard.


Fork this repo

Create a feature branch → git checkout -b feature/my-feature

Commit changes → git commit -m "Add my feature"

Push branch → git push origin feature/my-feature

Open a Pull Request 


Acknowledgements

Inspired by RoadsideCoder’s tutorial

Built with ❤️ using Next.js, Tailwind CSS, Prisma, Clerk, Inngest, and Gemini AI

📜 License

This project is licensed under the MIT License.
Feel free to use, modify, and distribute it with attribution.
