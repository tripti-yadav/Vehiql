Vehiql-AI Car Marketplace
An AI-powered full-stack car marketplace built with modern technologies including React 19, Next.js 15, Tailwind CSS, Supabase, Prisma, Gemini API, Clerk Authentication, Arcjet, and Shadcn UI. Users can list, discover, and analyze cars with the assistance of AI for smarter decisions.



🚀 Features
User Authentication: Secure login and registration using Clerk.

AI-Powered Listings: Generate car descriptions and recommendations using Gemini API.

Real-Time Updates: Instant updates on listings and user activities via Supabase.

Responsive UI: Modern and responsive design with Tailwind CSS and Shadcn UI.

Performance Optimization: Enhanced performance and security using Arcjet.

Advanced Filtering: Search and filter car listings by various parameters.

📁 Project Structure
bash
Copy code
/app         - Next.js 15 App Router pages and layouts
/components  - Reusable UI components built with Shadcn and Tailwind
/hooks       - Custom React hooks
/lib         - Utility functions and API helpers
/prisma      - Prisma schema and database migrations
/public      - Static assets
/styles      - Global Tailwind styles
🛠️ Setup Instructions
Prerequisites
Node.js (v18 or above)

PostgreSQL

Supabase account

Clerk account

Arcjet API key

Gemini API key (via Google AI)

Installation
Clone the Repository

bash
Copy code
git clone https://github.com/yourusername/ai-car-marketplace.git
cd ai-car-marketplace
Install Dependencies

bash
Copy code
npm install
Configure Environment Variables

Create a .env file in the root directory and add the following:

env
Copy code
DATABASE_URL=your_postgresql_connection_string
DIRECT_URL=your_direct_postgresql_connection_string
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
CLERK_SECRET_KEY=your_clerk_secret_key
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/onboarding
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/onboarding
GEMINI_API_KEY=your_gemini_api_key
ARCJET_KEY=your_arcjet_key
Set Up the Database

bash
Copy code
npx prisma generate
npx prisma migrate dev --name init
Run the Development Server

bash
Copy code
npm run dev
Open http://localhost:3000 in your browser to see the application.

📄 API Documentation
The application utilizes both server actions and Supabase API features. Core API functionalities include:

Authentication: Managed via Clerk.

Car Listings: Create, read, update, and delete car listings.

AI Features: Generate car descriptions and recommendations using Gemini API.

Real-Time Updates: Listen to changes in listings and user activities via Supabase.

Security: Implement rate limiting and bot protection using Arcjet.

🧰 Technologies Used
Frontend
React 19

Next.js 15 (App Router, Server Actions)

Tailwind CSS

Shadcn UI

Clerk Authentication

Arcjet (Performance & Security)

Backend & Services
Supabase (Database, Realtime, Storage)

Prisma ORM

PostgreSQL

Gemini API (Google AI)

