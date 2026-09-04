# Product Discovery Index

This directory is the product decision baseline for AI Teaching Canvas.

All documents marked **LOCKED** are considered the current source of truth unless a later product-discovery document explicitly supersedes a decision.

## Locked discovery documents

| Version | Document | Status | Purpose |
|---|---|---|---|
| V0.1 | [Product Definition](v0.1-product-definition.md) | LOCKED | Defines what the product is and is not |
| V0.2 | [Classroom Experience](v0.2-classroom-experience.md) | LOCKED | Defines the teacher journey and classroom surfaces |
| V0.3 | [Teaching Intelligence & Command Model](v0.3-teaching-intelligence-command-model.md) | LOCKED | Defines how teacher intent, context, and TeachingScene work |
| V0.4 | [Curriculum & Mathematics Intelligence](v0.4-curriculum-mathematics-intelligence.md) | LOCKED | Defines curriculum grounding, math generation, validation, and pedagogy |
| V0.5 | [Physical Classroom & Device Experience](v0.5-physical-classroom-device-experience.md) | LOCKED | Defines devices, pairing, display, resilience, touch, and classroom failure behavior |

## Product principles

1. **Teacher-first.**
2. **Software-first, hardware-agnostic.**
3. **Smart board is optional.**
4. **AI is a copilot, not the teacher.**
5. **LLM interprets; engines decide.**
6. **Backend owns authoritative state.**
7. **Generated classroom content is structured, not arbitrary HTML.**
8. **Mathematics is deterministically validated whenever possible.**
9. **Curriculum claims must be grounded in controlled, versioned curriculum data.**
10. **The classroom must remain usable when AI or internet availability degrades.**
11. **Student devices are optional, not a prerequisite for the core experience.**
12. **Privacy is minimized by default, especially for students.**

## Core product flow

```text
PREPARE
   ↓
PAIR
   ↓
TEACH
   ↓
ADAPT IN REAL TIME
   ↓
SAVE
```

## Core system concept

```text
Teacher voice / touch / ink
           │
           ▼
    Teaching Intent
           │
           ▼
    Classroom Context
           │
    ┌──────┼────────┐
    ▼      ▼        ▼
Curriculum Math    Lesson
 Engine    Engine  Context
    │      │        │
    └──────┼────────┘
           ▼
      TeachingScene
           │
           ▼
    Classroom Canvas
```

## Next phase

Do not continue broad discovery unless a material unknown blocks implementation.

Proceed to:

**MVP System Architecture & Technical Specification V0.1**
