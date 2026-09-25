# Chorus

A scalable, multilingual AI platform for aggregating citizen development
requests and surfacing infrastructure demand hotspots for national
policymakers. Built as a Digital Public Good.

## Why

Citizen feedback on development and infrastructure needs is scattered across
fragmented systems, making it hard for governments to align public spending
with what people actually need. Chorus consolidates that feedback and connects
it with national data to show where development attention is most needed.

## How it works

```
Citizen feedback  ->  Aggregation  ->  Analysis  ->  Demand hotspots  ->  Priorities  ->  Policymakers
(voice / text /       (unified          (joined with     (geographic        (ranked
 messaging apps,       store)            demographics,    clusters of        development
 many languages)                        infra indices,   unmet demand)      projects)
                                         investment
                                         plans)
```

## Architecture

- `src/chorus/ingestion` - intake from voice, text, and messaging channels
- `src/chorus/nlp` - language detection, translation, and classification
- `src/chorus/aggregation` - storage and deduplication of requests
- `src/chorus/analysis` - hotspot detection and project prioritization
- `src/chorus/api` - FastAPI service layer for policymaker-facing outputs

## Status

Early scaffold. Modules are placeholders under active development.

## License

MIT. See [LICENSE](LICENSE).
