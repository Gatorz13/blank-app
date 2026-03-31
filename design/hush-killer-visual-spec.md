# Hush Homepage Killer Visual Spec (Rebuilt)

## Message
**Same payment volume. Different visibility.**

Public rails convert repeated payments into inferable financial intelligence.
Hush preserves the same payment activity as private state and reveals only scoped receipts.

## Asset
- `landing/client/public/visuals/hush-killer-visual.svg`

## Composition
- Two large panels: **Public Rails** (left), **Hush** (right).
- Same payment pulse count enters both systems at the top of each panel.
- Left resolves into an exposed graph + red leakage endpoints.
- Right resolves into private state lanes + state object stack (`note`, `commitment`, `nullifier`) + one scoped receipt.
- Bottom outcomes:
  - `Public graph grows with time`
  - `Private state grows with time`

## Structural divergence (intentional)
- **Public side visual grammar:** network graph topology, clustering, outward leakage.
- **Hush side visual grammar:** containment + lane batching + private object accumulation.
- This avoids a mirrored/recolored chart and creates immediate outcome contrast.

## SVG group map (animation-ready)
- `canvas`
- `header`
- `panels`
- `shared-payment-input`
- `public-rails-side`
  - `public-relationship-graph`
  - `public-graph-nodes`
  - `public-cluster-emphasis`
  - `metadata-leakage`
  - `leakage-endpoints`
- `hush-side`
  - `hush-private-engine`
  - `hush-activity-lanes`
  - `hush-pulse-ticks`
  - `private-state-stack`
  - `state-continuity`
  - `scoped-receipt`

## Style constraints honored
- Background `#0B0F14`
- Teal `#0891b2`
- Red leakage only `#ef4444`
- Flat vector only
- No charts, legends, report boxes, gradients, glow, blur, or 3D

## Rive transitions (3–4)
1. Payment pulses enter both panels equally.
2. Public graph densifies and leakage endpoints activate.
3. Hush lanes fill and private state stack accumulates.
4. Scoped receipt appears on demand.
