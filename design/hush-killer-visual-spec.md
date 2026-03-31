# Hush Killer Visual Spec (Structure Divergence Refinement)

## Core message
**Same payment activity. Different visible structure.**

- **Public Rails:** repeated transfers resolve into an exposed, readable relationship graph.
- **Hush:** repeated transfers resolve into private state accumulation (notes, commitments, nullifiers) with scoped receipts.

## Asset
- `landing/client/public/visuals/hush-killer-visual.svg`

## Key refinement in this version
The two panels no longer share the same visual grammar.

- Left uses **actor-to-actor graph topology** with increasing cluster density and leakage endpoints.
- Right uses **batch/state topology** (ingress, epoch batches, private objects, continuity links, scoped receipt), avoiding a recolored public graph pattern.

## Composition
1. **Shared constants (for fair comparison)**
   - Same actor set.
   - Same epoch timeline (`t0→t4`).
   - Same transaction activity volume motif.

2. **Public Rails panel**
   - Dense transfer edges + densification overlays.
   - Cluster envelopes intensify over time.
   - Red leakage paths terminate at external endpoints.
   - Outcome: exposed relationship graph compounds.

3. **Hush panel**
   - Activity enters epoch batch lanes.
   - Equal per-epoch activity shown as tick stacks.
   - State resolves into `note`, `cm`, `nf` objects with continuity links.
   - Scoped receipt shown without exposing full graph.
   - Outcome: private state compounds while relationship graph remains non-public.

## Style constraints honored
- Flat vectors only
- Background `#0B0F14`
- Teal accent `#0891b2`
- Red leakage `#ef4444`
- White / muted gray / cyan text only
- No gradients, glow, blur, 3D, or decorative effects

## Rive transitions (3–4)
1. Show equal activity baseline in both panels.
2. Public panel densifies + leakage endpoints activate.
3. Hush panel batch lanes fill and private objects accumulate.
4. Scoped receipt appears as selective disclosure.
