# PROMPT ENGINEERING 


                 ┌─────────────┐
                 │    INPUT    │
                 │  (Raw Task) │
                 └──────┬──────┘
                        │
                        ▼
    ╔════════════════════════════════════════╗
    ║         PROMPT CONSTRUCTION            ║
    ║                                        ║
    ║  ┌─────────────┐  ┌─────────────────┐  ║
    ║  │  ROLE /     │  │   INSTRUCTIONS  │  ║
    ║  │  PERSONA    │  │  • Be specific  │  ║
    ║  │  "Act as…"  │  │  • Use steps    │  ║
    ║  └─────────────┘  │  • Set format   │  ║
    ║                   └─────────────────┘  ║
    ║  ┌──────────────────────────────────┐  ║
    ║  │          CONTEXT / EXAMPLES      │  ║
    ║  │  Background ─── Few-shot Samples │  ║
    ║  │  Constraints ── Output Format    │  ║
    ║  └──────────────────────────────────┘  ║
    ╚════════════════════════════════════════╝
                        │
                        ▼
    ╔════════════════════════════════════════╗
    ║            LLM / AI MODEL              ║
    ║                                        ║
    ║   Tokenize ──► Attend ──► Generate     ║
    ║       ↑                        │       ║
    ║       └───── Context Window ───┘       ║
    ╚════════════════════════════════════════╝
                        │
                        ▼
                ┌─────────────┐
                │   OUTPUT    │
                │  (Response) │
                └─────────────┘