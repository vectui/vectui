# Contributing to VectUI

Thank you for helping build Ghana’s open-source Design Engineering ecosystem! Whether you are submitting your very first pull request or architecting complex ARIA components, you are welcome here.

---

## 🎨 Track A: UI/UX & Vector Design Contributors

All icons in `@vectui/icons` follow strict grid physics so they render crisply across all screen DPIs and low-end mobile devices:

### Vector Grid Rules
1. **Canvas Size:** `24px × 24px` frame.
2. **Live Active Area:** `20px × 20px` (maintain a `2px` outer padding boundary on all sides).
3. **Stroke Weight:** Uniform `2px` stroke width.
4. **Caps & Joins:** Round line caps (`stroke-linecap="round"`) and round line joins (`stroke-linejoin="round"`).
5. **Color Inheritance:** Use `stroke="currentColor"` (no hardcoded hex fills on stroke icons).
6. **Naming Convention:** Use lowercase `kebab-case` (e.g., `momo-cash-out.svg`, `susu-box.svg`, `trotro.svg`, `asanka.svg`).

### How to Submit an Icon
1. Duplicate the official **VectUI Figma Master File** and draw your icon inside a `24×24px` frame.
2. Outline/clean paths so there are zero overlapping sub-paths or hidden clip masks.
3. Export as SVG and place it inside `packages/icons/src/raw/<icon-name>.svg` (or attach the SVG to an Icon Request issue if you prefer a maintainer to run the build step).
4. Open a Pull Request targeting `main`.

---

## 💻 Track B: Frontend & Design Engineering Contributors

### Monorepo Structure
- `apps/docs` — Next.js documentation & interactive copy-paste registry site
- `packages/icons` — `@vectui/icons` (SVGR + SVGO build pipeline)
- `packages/tokens` — `@vectui/tokens` (Style Dictionary token compiler)
- `packages/cli` — `vectui` CLI distribution tool
- `registry/ui` — Raw TypeScript + Tailwind UI primitives

### Code & Performance Standards
- **Low-Bandwidth First:** Tree-shaken icons must remain under **`1.5KB`** with zero runtime dependencies.
- **Accessibility:** All interactive registry components (`MoMoDrawer`, `PinInputGrid`, etc.) must use WAI-ARIA compliant primitives (Radix UI) with full keyboard navigation and screen reader labels.
- **TypeScript Strictness:** All components and utilities must pass strict TypeScript checks without `any` types.

### Submitting a Code PR
1. Fork the repository and create a feature branch:
   ```bash
   git checkout -b feat/add-momo-drawer
   ```
2. Run `pnpm build` and `pnpm lint` to ensure all workspace packages compile cleanly.
3. Open a Pull Request against `main` with a clear description (and screenshot/GIF if updating UI).