
                  User Query
                       │
                       ▼
                Multi-Agent System
                       │
        ┌──────────────┼──────────────┐
        ▼              ▼              ▼
   Semantic       Memory Scoring   Retrieval
 Checkpointing    Confidence+Utility
        │              │
        └──────┬───────┘
               ▼
      Memory Lifecycle Manager
      (Promote / Keep / Archive)
               │
               ▼
        Context for LLM
               │
               ▼
         Final Response
