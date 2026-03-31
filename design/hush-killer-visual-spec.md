# Hush Homepage Killer Visual Spec (Refined)

## Objective
Demonstrate a single high-value proposition with institutional clarity:

- **Same actors and same payment throughput** on both rails.
- **Public rails**: relationship graph and metadata inference surface compound over time.
- **Hush**: system activity compounds private state, while disclosure stays scoped.

## Assets
- `landing/client/public/visuals/hush-killer-visual.svg`
- `design/hush-killer-visual-spec.md`

## Composition (Desktop 1600×900)

### 1) Hierarchy
- Shared headline anchors the comparison first.
- Two symmetric panels support direct, investor-grade side-by-side reading.
- Clear top-level labels: **Public Rails** vs **Hush**.

### 2) Temporal clarity
- Both panels include explicit epoch columns `t0 → t4` with column banding.
- Column banding gets progressively stronger to emphasize time and accumulation.
- Transaction paths cross all epochs to signal equivalent ongoing volume.

### 3) Shared actor parity
Same actor row appears on both sides, same order:
- issuer
- Alice
- Bob
- merchant
- payroll
- treasury
- auditor

## Public Rails side behavior

### What increases over time
1. Baseline payment paths (constant throughput)
2. Cross-epoch relationship links (density increases by epoch group)
3. Metadata leakage branches in red
4. Inference-risk index bars (`t0` to `t4`) that visibly grow

### Inferable metadata labels
- balance
- timing
- counterparties
- frequency
- settlement

### Interpretation
Even without payload decryption, repeated transparent edges and metadata cadence create a progressively inferable payment graph.

## Hush side behavior

### What increases over time
1. Baseline payment paths (same throughput as left)
2. Epoch state objects (`note_*`, `cm_*`, `nf_*`) with continuity links
3. Operational system lane (`proof gen → state root → commit → nullify → finalize`)
4. One scoped auditor receipt as selective disclosure

### Interpretation
Activity remains high and system-like, but external visibility accumulates as controlled state transitions rather than public relationship topology.

## Style constraints (implemented)
- Background: `#0B0F14`
- Teal accent: `#0891b2`
- Red leakage only: `#ef4444`
- Text: white/muted gray/cyan only
- Flat vectors only
- No gradients / no glow / no blur / no 3D

## SVG group architecture
Top-level:
- `canvas`
- `header`
- `panels`
- `temporal-rails`
- `actors`
- `public-rails-side`
- `hush-side`
- `legend`

Animation-ready subgroups:
- `public-transaction-volume`
- `public-relationship-accumulation`
- `metadata-leakage`
- `inference-risk-index`
- `private-state-system`
- `state-transition-bus`
- `system-lane`
- `scoped-auditor-receipt`

## Rive transition plan (3–4 states)
State machine: `VisibilityComparison`

1. **State A — Throughput parity**
   - Draw both sides’ payment paths together (t0→t1).
2. **State B — Public inferability compounding**
   - Reveal epoch-group relationship links + red leakage + risk index growth.
3. **State C — Private state compounding**
   - Step reveal `note/cm/nf` columns and transition bus.
4. **State D — Scoped disclosure event**
   - Animate receipt path to auditor only; keep global graph hidden.

## Notes for implementation
- Asset is intentionally diagrammatic and avoids decorative motifs.
- Spacing prioritizes label legibility and timeline readability for future responsive adaptation.
