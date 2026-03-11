# Draft: Site de Geografia para o ENEM

## Requirements (confirmed)
- Provide **all** types of educational content (text, images, diagrams, videos, interactive maps, quizzes, simulados, questões de prática, etc.) – as many units/chapters as necessary to cover the ENEM geography syllabus.
- Target audience: **estudantes do ensino médio** preparing for the ENEM.
- Required features (all of the following):
  - Full‑text search across content
  - Quiz engine with automatic correction and score tracking
  - Bookmark/favorites system for students
  - Blog/news section for ENEM updates
  - Social‑share buttons
  - Responsive design (desktop + mobile)
  - Optional login (public‑only mode will be used; login not required)
- Tech stack:
  - Modern static site generator based on **React/Next.js** with **TypeScript**
  - UI components from **shadcn/ui** (Tailwind‑CSS)
  - Deployed on **Vercel** (fallback to GitHub Pages if needed)
- Design: No existing brand assets; will be inspired by leading ENEM prep sites (e.g., Khan Academy, Brasil Escola, Stoodi, Descomplica).
- Testing: **Test‑after** approach (implement first, then add automated tests).
- Timeline: MVP in **2 hours** (quick prototype).
- Maintenance: Owner (you) will update content manually; no admin panel required.

## Technical Decisions
- Use **Next.js (App Router)** for static generation (SSG) with incremental static regeneration if needed.
- Store content in **Markdown files** under `content/` (easy to edit, version‑controlled).
- Generate quizzes from structured YAML/JSON files.
- Use **Playwright** for end‑to‑end UI verification; **Vitest** for unit tests.

## Research Findings
- shadcn/ui integrates smoothly with Next.js and Tailwind, providing accessible components.
- Vercel offers free tier sufficient for static sites with custom domains.

## Open Questions
- None – all decisions made.

## Scope Boundaries
- **INCLUDE**: All educational content, interactive features, search, quizzes, blog, responsive UI.
- **EXCLUDE**: Paid premium subscription features, complex user dashboards, real‑time chat support.
