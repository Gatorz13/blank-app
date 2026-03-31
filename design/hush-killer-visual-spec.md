# Hush Killer Visual Spec (3-second Read Version)

## Core message
**Same payment volume. Different visibility.**

- Left: transparent rails compound an inferable relationship graph.
- Right: Hush compounds private state with scoped disclosure.

## Asset
- `landing/client/public/visuals/hush-killer-visual.svg`

## What changed in this refinement
- Reduced on-canvas copy to headline, panel labels, actor names (once), and two short outcomes.
- Removed legends, large explanatory callouts, and process-label clusters.
- Increased visual hierarchy: larger headline, stronger panel labels, cleaner spacing.
- Kept temporal readability with explicit `t0→t4` columns on both sides.

## Composition
1. **Shared timeline scaffolding**
   - Epoch columns `t0→t4` on both sides.
   - Identical actor rows and equal transaction line density.

2. **Public Rails side**
   - Repeated payment paths.
   - Layered graph-density links that increase by epoch.
   - Red leakage tendrils exiting to external points.
   - Outcome line: inferability grows with time.

3. **Hush side**
   - Same payment throughput motif.
   - Private state rows (`note`, `cm`, `nf`) that accumulate by epoch.
   - State continuity links across epochs.
   - One scoped auditor receipt.
   - Outcome line: private state grows with time.

## Visual constraints honored
- Flat vectors only
- Background `#0B0F14`
- Teal accent `#0891b2`
- Red leakage `#ef4444`
- White/muted gray/cyan text only
- No gradients / glow / blur / 3D / decorative effects

## Rive transitions (3–4)
1. Throughput parity appears on both sides.
2. Public graph density + red leakage compounds.
3. Hush private state blocks and links compound.
4. Scoped auditor receipt toggles in.
