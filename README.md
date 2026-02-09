# Emotional Mirror (Web MVP)
A privacy-first, opt-in self-awareness companion: chat + a short (30s) camera session that gives a gentle, non-clinical “emotional mirror” (e.g., possible tension/stress) and guides the user into reflection.

> **Not therapy. Not a medical device. No diagnosis.**

## Why this exists
Many people say “I’m fine” while their body shows signs of tension or stress. This project helps users notice that mismatch and choose a short reflection flow to regain clarity and control.

## MVP scope (Web)
### Included
- Chat UI (session-based)
- **Opt-in** “Self-Awareness Session (30s)” using the camera (user-initiated only)
- Ephemeral processing (no raw video stored by default)
- Output: 3–4 high-level states + confidence (e.g., calm/tension/stress/fatigue)
- Reflection flow (5–7 prompts) after results

### Not included (MVP)
- No continuous monitoring / background camera use
- No medical claims, diagnosis, or treatment
- No storing raw video/audio frames
- No payments, no notifications, no long-term analytics (yet)

## Safety & privacy principles
- Camera is **OFF by default** and runs only after explicit user action
- Session is time-limited (default: 30s) and user can stop anytime
- Default: do not store raw video; store only aggregated signals (optional)
- Users can delete their stored data
- Crisis handling: if user indicates self-harm risk, the assistant provides crisis resources and encourages contacting professionals

## Tech (planned)
- Frontend: Next.js (React)
- Backend: FastAPI (Python)
- DB: PostgreSQL (or Supabase)
- CV signals: MediaPipe face landmarks (MVP) + simple heuristics
- LLM: dialogue + guardrails + structured prompts

## Repo structure
- `/frontend` – Next.js web app (chat + camera session)
- `/backend` – FastAPI API (sessions, optional storage)
- `/docs` – product spec, UX flow, privacy/safety notes

## Quickstart (placeholder)
Coming soon.

## Roadmap
- v0.1: chat + consented camera session + basic results + reflection flow
- v0.2: user profile (patterns over time) + export/delete
- v0.3: optional voice signals + improved signal model

## License
TBD
