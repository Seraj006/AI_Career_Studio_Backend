# AI_Career_Studio_Backend

Production-ready Node.js, Express, TypeScript, and Prisma backend for AI Career Studio (Job-Search Workspace for Indian Job Seekers).

# Tech Stack & Architecture
- Runtime & Language: Node.js + Express (ES Modules) + TypeScript
- Database & ORM: MongoDB Atlas with Prisma ORM
- Authentication: JWT (JSON Web Tokens, 7-day expiry) with bcrypt password hashing (10 salt rounds)
- Validation: Zod schema middleware for request body, query, and params
- Security: Helmet, CORS (allowing http://localhost:5173 and http://localhost:5174), strict rate limiting for auth endpoints
- AI & Analysis: LLM integration (Anthropic Claude / Gemini / OpenAI) with intelligent rule-based heuristic fallback
- File Parsing: Multer memory storage (5MB max) + pdf-parse + mammoth (DOCX)
- Testing: Vitest + Supertest

# Getting Started

## 1. Install Dependecies
```bash
npm install
```

##  2. Configure Environment
Copy `.env.example` to `.env`:
Key configuration variables:
- ` PORT: Set to ` ` 5000 ` (matches frontend default VITE_API_URL=http://localhost:5000).
- ` DATABASE_URL: MongoDB Atlas connection string.
- ` JWT_SECRET: Secure string of at least 32 characters.
- ` ANTHROPIC_API_KEY / ` ` GEMINI_API_KEY /` ` OPENAI_API_KEY: ` Optional; an intelligent heuristic fallback analyzer is active if comitted.
