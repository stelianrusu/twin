# Claude Instructions — Personal Preferences

## Background
I am a software engineer with strong experience in **Azure** and **.NET**. I am learning Python, FastAPI, and AI-integrated SaaS patterns. Use Azure/.NET analogies when introducing new concepts — this is my primary mental model.

Examples of useful analogies:
- FastAPI ≈ ASP.NET Minimal APIs
- FastAPI middleware ≈ ASP.NET middleware pipeline
- Clerk ≈ Azure AD B2C
- Vercel ≈ Azure Static Web Apps + Azure Functions
- AWS App Runner ≈ Azure Container Apps
- Python virtual environment (`venv`) ≈ NuGet package isolation per project
- Pydantic models ≈ C# record types / data annotations

---

## AI Provider
Always use **Anthropic** (Claude models via the Anthropic SDK), never OpenAI — even if the source material, lab guide, or reference repo specifies OpenAI. Translate all OpenAI-specific code to Anthropic equivalents.

---

## Teaching and Execution Style

### Step-by-step approach — always follow this:
1. **Explain WHAT we are building** and WHY before writing any code
2. **One logical unit at a time** — one file, one concept, one endpoint
3. **After each step, pause and confirm** before proceeding to the next
4. **No code dumps** — never output multiple files at once without explanation
5. **Show the full file** when creating something new, not just a snippet

### Explanations:
- Explain new tools, libraries, or patterns as if I have not seen them before in the Python/JS ecosystem
- Draw the Azure/.NET analogy first, then explain the Python/JS equivalent
- When a decision is made (e.g., why Pages Router over App Router), explain the tradeoff explicitly

---

## Code Style
- Use TypeScript (not plain JavaScript) for all frontend code
- Do not add comments explaining WHAT the code does — only add comments for non-obvious WHY

---

## Project Structure Expectations
- The spec lives in `week2/` (relative to this file's directory). At the start of each session, read all files there (`day1.md` through `day5.md`) to understand the full scope, then ask me which day we are working on before doing anything else.
- Do not introduce abstractions or refactors beyond what the current task requires
- Do not add error handling for scenarios that cannot happen in the current context

---

## Preferred Workflow
- Read the task list or spec file at the start of each session
- Confirm current progress before starting new work
- Flag any deviation from the spec before implementing it
