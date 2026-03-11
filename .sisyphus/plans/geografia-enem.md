# Plano: Site de Geografia para o ENEM

## TL;DR
> Criação de um site estático completo para ensino de Geografia focado no ENEM, com conteúdo multimídia, quizzes, busca, marcações e blog, usando Next.js + shadcn/ui, hospedado no Vercel.

## Context
- **Objetivo**: oferecer material didático completo para estudantes do ensino médio que se preparam para o ENEM.
- **Público‑alvo**: estudantes do ensino médio.
- **Tecnologia**: Next.js (App Router) + TypeScript, shadcn/ui, TailwindCSS, Vercel (fallback GitHub Pages).
- **Conteúdo**: textos, imagens, diagramas, vídeos, mapas interativos, quizzes, simulados, questões de prática.
- **Manutenção**: será feita manualmente pelo proprietário.

## Work Objectives
- Gerar estrutura do projeto (Next.js + shadcn/ui).
- Criar sistema de conteúdo baseado em Markdown.
- Implementar busca full‑text (client‑side).
- Desenvolver engine de quiz com correção automática.
- Adicionar funcionalidade de bookmark/favoritos.
- Construir blog de atualizações do ENEM.
- Garantir responsividade e SEO.
- Deploy automático no Vercel.

## Verification Strategy
- **Teste automatizado**: Vitest unit tests + Playwright e2e para UI.
- **Critério de aceitação**: Todas as páginas carregam sem erros, quizzes avaliam respostas corretas, busca retorna resultados esperados, favoritos persistem em `localStorage`.
- **Agente‑executado QA**: cada tarefa inclui cenários de happy‑path e de erro.

## Execution Strategy
- **Paralelização**: dividir em ondas (waves) de tarefas independentes.
- **Wave 1 – Fundamentos**: scaffolding, configuração Tailwind, shadcn/ui, rotas iniciais.
- **Wave 2 – Conteúdo**: estrutura de Markdown, carregamento, renderização.
- **Wave 3 – Funcionalidades**: busca, quiz, favoritos, blog.
- **Wave 4 – Testes & Deploy**: Vitest, Playwright, CI, Vercel deploy.

---

## TODOs

---

## Final Verification Wave
- [ ] F1. **Plan Compliance Audit** – Oracle
- [ ] F2. **Code Quality Review** – lint, tsc, tests
- [ ] F3. **Real Manual QA** – Playwright end‑to‑end
- [ ] F4. **Scope Fidelity Check** – verify no extra features

## Commit Strategy
- Commits atomizados por tarefa, mensagens `type(scope): description`.

## Success Criteria
- Site publicado no Vercel, sem erros de console, com todas as funcionalidades listadas operacionais.
