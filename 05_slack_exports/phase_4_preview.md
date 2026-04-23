# Phase 4 — Zoom 1 + meeting notes (staging)

**Slack channel:** `C0A6ZJ9NH5E`  
**New parent:** Phase 4 only (not Phase 1/2/3 `thread_ts`).

## Google Doc #2

- Title: `GeomDeent — Meeting Notes 2026-04-22`
- Created via Composio `GOOGLEDOCS_CREATE_DOCUMENT_MARKDOWN`; URL posted in thread.

## Resolved decisions (for commits / cp_current)

1. **Leakage reporting:** Primary scalar = **KL(clean ‖ intervened)** on next-token distribution over a fixed probe set. Same table includes **Δentropy** and **repetition / bigram repeat** (Brent). Chris keeps **recover + judge-flip** as tertiary diagnostics in the leakage vector.
2. **Layer scope:** Alex implements **per-layer ladder at L**; Brent adds **smear check** — same semantic probe on residual at **L and L+2** after orthogonalize; log cosine drift; flag “smeared coordinate” if drift exceeds threshold (TBD in pilot).
3. **Toy model:** **Qwen2.5-0.5B-Instruct** as default shared small model; fall back to **TinyLlama-1.1B** only if VRAM blocks; freeze tokenizer + chat template across RAs.

## Slack (posted)

**Phase 4 parent `ts`:** `1776920017.706679`

**Google Doc #2:** https://docs.google.com/document/d/18485IOiDVvfDY8qezUAd-P9HSsXYiScZ6NZR17NDLJE/edit  
**documentId:** `18485IOiDVvfDY8qezUAd-P9HSsXYiScZ6NZR17NDLJE`

## Git (GeomDeent repo)

| Branch | Commit | Author | Notes |
|--------|--------|--------|-------|
| `main` | `a3a76d8` | Tyler `<treed.lab30@gmail.com>` | `phase_4_preview` (+SHA table), `06_decisions/...zoom1.md`, `cp_current` (tip after P4) |
| `RA1` | `187e1bf` | Alex `<researchassistant111@outlook.com>` | `research-log/phase4_zoom1.md` (post-merge) |
| `RA2` | `4ab4e52` | Brent `<researchassistant222@outlook.com>` | `phase4_zoom1` content fix after merge |
| `RA3` | `b135b77` | Chris `<researchassistant333@outlook.com>` | `research-log/phase4_zoom1.md` |

### Thread index

| `ts` | Who | Summary |
|------|-----|---------|
| `1776920017.706679` | Tyler | Parent — quick sync, parking lot topics |
| `1776920035.833649` | Tyler | `[zoom 1 — transcript]` + agenda |
| `1776920041.354759` | Alex | KL headline + ΔH/repeat columns; ladder-at-L |
| `1776920044.023989` | Brent | repetition column; L/L+2 residual probe |
| `1776920045.029349` | Chris | third tier ok; asks smeared cutoff |
| `1776920046.693739` | Tyler | thresholds from pilot tails |
| `1776920050.570919` | Chris | yeah ok |
| `1776920051.598449` | Brent | L+2 enough on 0.5B |
| `1776920052.443289` | Alex | L+2 works |
| `1776920053.403859` | Tyler | toy model + freeze templates |
| `1776920057.533599` | Alex | VRAM smoke test |
| `1776920059.589139` | Tyler | decisions locked recap |
| `1776920060.813379` | Tyler | doc link |
| `1776920061.890269` | Tyler | reply only if blocked |
| `1776920063.094049` | Brent | copy — stub hooks |
| `1776920063.997609` | Chris | align steg table shape |
