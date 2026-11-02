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

## Install Dependecies

