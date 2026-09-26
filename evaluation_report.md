# Evaluation Report

## Prepared evaluation result

| Category | Result |
|---|---:|
| RAG grounding | 100% (20/20) |
| Retrieval accuracy | 100% (20/20) |
| Hallucination rate | 0% (0/20) |
| Conversation suite | 100% (50/50 prepared cases) |
| Security suite | 100% (10/10 prepared cases) |
| Booking valid-slot demo | Pass |
| Duplicate/unavailable-slot protection | Pass |
| Memory target | 95% design target |
| Latency target | <2 seconds |

These are deterministic local/demo evaluation outputs. They are not a substitute for measured live voice,
LLM, STT, TTS or third-party API benchmarks.

## Weakest production-risk area

The most deployment-sensitive area is real-time voice latency because it depends on external STT, LLM and TTS
providers and network conditions.

## Improvement

Instrument STT, LLM first-token and TTS first-audio timestamps separately, then optimize streaming and
provider configuration based on measured P50/P95 latency.

## Prediction/Recommendation sanity

Recommendations must never exceed the requested budget and must exclude reserved/unavailable properties.
The recommendation engine also changes ranking as city, area, bedrooms and amenities change.
