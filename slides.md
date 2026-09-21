# Stakeholder Slide Deck

## Slide 1 — Real Estate UrduLish AI Voice Agent
Voice + RAG + Recommendations + Scheduling

## Slide 2 — Business Problem
- High inbound call volume
- inconsistent first response
- repetitive property questions
- manual appointment coordination
- need for UrduLish customer experience

## Slide 3 — Product
- natural voice
- context memory
- verified property answers
- recommendations
- objection handling
- calendar/email/CRM workflows

## Slide 4 — Architecture
Telephony → STT → FastAPI → LangGraph → SQL/RAG/Recommendation/Calendar/Email/CRM → TTS

## Slide 5 — Knowledge & Grounding
Structured data for exact facts.
Vector retrieval for brochures, descriptions and FAQs.
No guessing when evidence is missing.

## Slide 6 — UrduLish Experience
Warm Pakistani persona.
Natural acknowledgements and fillers.
Short phone-friendly turns.
No literal translation.

## Slide 7 — Workflow Automation
Call → Intent → Property Match → Appointment → Calendar → Email → CRM

## Slide 8 — Security
Prompt injection defense.
No internal prompt/secret disclosure.
No fake appointments.
No unavailable property recommendations.
Human escalation.

## Slide 9 — Evaluation
20 RAG cases.
50 conversation cases.
10 security cases.
Prepared demo results: 100% pass on local deterministic suite.

## Slide 10 — Deployment & Roadmap
Docker + FastAPI.
Production database/vector DB.
Monitoring and backups.
Roadmap: WhatsApp, SMS, CRM, multilingual, analytics, lead scoring, live property feed.
