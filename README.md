# Emotional Mirror (MVP)
Voluntary (opt-in) self-awareness companion: chat + short camera-based session to help users reflect on emotional tension/stress.
Not a medical device. Not therapy. No diagnosis.

## What this is
A privacy-first well-being tool that helps users notice possible signs of stress/tension and guides them through gentle reflection.

## Core MVP features
- Chat interface (session-based context)
- "Self-Awareness Session (30s)" camera mode (user-initiated only)
- On-device / ephemeral processing: no video stored
- Outputs 3–4 high-level states (e.g., calm / tension / stress / fatigue) + confidence
- Follow-up reflection prompts (no clinical claims)

## What this is NOT
- Not therapy, not a substitute for professional help
- No diagnosis, no medical claims
- No continuous monitoring, no background camera use
- No hidden recording

## Privacy & Safety
- Camera is OFF by default and only runs after explicit user action
- Default: do not store video/audio
- Only store aggregated numeric signals (optional, can be disabled)
- Users can delete their data
- If user indicates self-harm risk: provide crisis resources and encourage contacting professionals

## Tech (planned)
- Frontend: Next.js (React) + WebRTC getUserMedia
- Backend: FastAPI + PostgreSQL (user profile) + Redis (sessions)
- CV signals: MediaPipe face landmarks (MVP) + heuristic stress/tension indicators
- LLM: dialogue + structured prompts + guardrails

## Repo structure
- `/frontend` – web UI (chat + camera session)
- `/backend` – API, user state, session logic
- `/docs` – product spec, UX flows, safety notes

## Getting started (placeholder)
Coming soon.

## Roadmap
- v0.1: chat + camera session + basic signals + reflection flow
- v0.2: user profile (patterns over time) + export/delete data
- v0.3: voice signals (optional) + improved feedback quality

## License
TBD
