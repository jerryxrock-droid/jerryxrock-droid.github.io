---
layout: single
title: Projects
permalink: /en/projects/
author_profile: false
---

## 🎯 Featured Projects

### Cariad (VW Group) · Data Collection Product
**2023.07 – Present · Million-Vehicle Platform**

End-to-end ownership of vehicle-side data collection product. Designed the metrics taxonomy, collection frequency, data quality monitoring, and PIPL-compliant data flow.

- **Outcome**: Defined the "data usability score" loop from analytics team back to product spec. Crossed vehicle/cloud/privacy/legal silos.
- **Stack thinking**: PM-side is a "data marketplace" problem — what's collected, how it's labeled, who consumes it, what's the SLA.
- **For AI PM**: Mirrors the "data flywheel" problem in AI products (collect → label → train → eval → feedback).

### Ford China · In-Car Voice Product (SYNC+)
**2021.09 – 2023.07**

Owned Ford China's voice product UX. Defined voice intent taxonomy (navigation / media / vehicle control), worked with Tencent and Baidu voice engines.

- **Outcome**: Shipped voice control for 12+ in-car intents across 3 vehicle models.
- **For AI PM**: Voice intent classification is a classic NLU problem. The UX principles translate directly to LLM chat UX.

### SAIC VW · Remote Vehicle Control
**2018.01 – 2021.09**

Remote vehicle control features (lock/unlock, AC pre-cool, find my car) for SAIC VW's connected car app. Worked with Bosch and Huawei car BU.

- **Outcome**: Defined the mobile command protocol and security model. Shipped to 8 SAIC VW models.
- **For AI PM**: API design for mobile-command systems is the same discipline as designing AI tool-use APIs.

---

## 🛠 Side Projects (iOS Development)

I build iOS apps to **understand technology teams' thinking** — not to become an indie developer. The goal is to bridge PM and engineering in my next AI PM role.

### ZhiTong (职通) — AI-Powered Job Search App
**2025 · 5-tab SwiftUI app · SQLite**

Job matching app with weighted skill scoring (0-100 match score, 3 tiers: qualified / reachable / long-term). Includes dynamic lesson cards (3-card structure: concept / standard / test) per skill.

- **Architecture**: MVVM with `DataStore` (singleton) as the business core, `@StateObject` for state injection.
- **Persistence**: SQLite (jobs/assessments/learning plans) + UserDefaults (learning progress).
- **Source**: [github.com/jerryxrock-droid/ZhiTong](https://github.com/jerryxrock-droid/ZhiTong)

### Xuanjing (玄镜) — Deterministic Zodiac/MBTI/Tarot App
**2024 · 32 SwiftUI files · MVVM · UserDefaults**

Combines zodiac + MBTI + tarot into a daily self-exploration app. Uses a **deterministic seed algorithm** (LCG + `&*`/`&+` for overflow safety) so the same user sees the same cards all day.

- **Why deterministic**: Random card draw makes users think "this app is inaccurate". Deterministic = "this app is consistent". UX choice.
- **Source**: [github.com/jerryxrock-droid/Xuanjing](https://github.com/jerryxrock-droid/Xuanjing)

### Still — Sleep / Breathing Audio App
**2024 · SwiftUI + SwiftData · 20 files**

Sleep + breathing audio app. 4-stage breathing rhythm (4-4-6-2 pattern), 5 ambient sound types (Brown / White / Rain / Ocean / Forest) generated in real-time via `NoiseGenerator`.

- **Architecture**: `LFOModulator` for LFO-based audio modulation, `SleepTracker` for accelerometer-based sleep estimation.
- **Storage**: SwiftData with `Thought` / `SleepSession` / `SleepReport` schema (3 entities, cascade delete).

### ShiMo (拾墨) — Classical Poetry SRS App
**2024 · CoreData + SQLite FTS5 · 43 files**

Classical poetry learning app with FSRS-style spaced repetition (mastered=7d / notFamiliar=3d / notMastered=1d intervals) and SQLite FTS5 full-text search across 300+ poems.

- **Tech**: `FTSDatabase` for FTS5 (poemId / title / author / dynasty / fullText / category schema), `ExerciseEngine` for fill-in-the-blank exercise (3 difficulty levels: 20%/35%/55% blank ratio).

### More Projects

- **MemoMiniApp** — Multi-modal memo with voice-to-text, translation (mock), Face ID
- **StarGravity** — Astrology app (CoreData — currently has a P0 data-loss issue)
- **FitEat** — Fridge-based recipe recommendation (SQLite + howtocook dataset)
- **FitRock** — Fitness tracker (MVVM + HealthKit + 4 haptic types)
- **GuitarBook** — Chord library + song editor (UserDefaults + CoreData scaffold)

📂 **All 10 iOS projects analyzed**: see [code atlas PDF](https://github.com/jerryxrock-droid/jerryxrock-droid.github.io/raw/main/assets/iOS-项目代码图谱-2026-06-17.pdf) (84 pages, 9.8MB, 46 mermaid diagrams).

---

## 📝 Writing

- [Why I'm Pivoting to AI PM (2026 H1)]({{ '/en/blog/why-ai-pm-pivot/' | relative_url }}) — 5400 words, the full story

---

<!-- Language switcher -->
<div style="text-align: center; margin-top: 3rem; padding: 1rem; border-top: 1px solid #333;">
  <a href="/projects/" style="color: #D4A843; text-decoration: none;">← 中文版</a>
</div>
