<div align="center">
  <h1>VectUI</h1>
  <p><strong>Ghana’s open-source Design Engineering collective & localized UI asset ecosystem.</strong></p>
  <p>
    <a href="https://github.com/vectui/vectui/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT License" /></a>
    <a href="https://github.com/vectui/vectui/blob/main/CONTRIBUTING.md"><img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" alt="PRs Welcome" /></a>
  </p>
</div>

---

## 🌍 What Is VectUI?

**VectUI** is an open-source Design Engineering ecosystem and community initiative built in Ghana for the African tech ecosystem. We unite UI/UX designers and frontend engineers to bridge Figma design systems with clean, accessible, low-bandwidth production code—eliminating the "Default UI" debt caused by Western-centric component libraries.

### 📦 Ecosystem Packages

| Package | Description | Status |
| :--- | :--- | :--- |
| **`@vectui/icons`** | 30+ Ghanaian-focused vector icons on a strict `24×24px` grid (`2px` uniform stroke, `<1.5KB` per icon). Ships as raw SVGs and tree-shakable React components. | 🚧 Phase 1 |
| **`@vectui/tokens`** | Style Dictionary token engine syncing Figma Variables directly into CSS variables and Tailwind CSS presets (`--color-momo-yellow`, `--color-kente-gold`, `--color-asanka-clay`). | 🚧 Phase 2 |
| **`@vectui/registry`** | Copy-paste CLI registry (`npx vectui add`) delivering accessible TypeScript + Tailwind UI primitives (`MoMoDrawer`, `PinInputGrid`, `OfflineBanner`) directly into your repo. | 🚧 Phase 3 |

---

## 🚀 Quick Start (Local Development)

### Prerequisites
- **Node.js** `>= 20.0.0`
- **pnpm** `>= 9.0.0` (`npm install -g pnpm`)

### Setup
```bash
# 1. Clone the repository
git clone [https://github.com/vectui/vectui.git](https://github.com/vectui/vectui.git)
cd vectui

# 2. Install workspace dependencies
pnpm install

# 3. Build all packages (@vectui/icons, @vectui/tokens)
pnpm build

# 4. Start the local docs & registry app
pnpm dev
```

---

## 🤝 Contributing

We welcome contributing members across both **UI/UX Vector Design** and **Frontend / Design Engineering**—whether you are a seasoned builder or making your very first open-source pull request.

Read **[CONTRIBUTING.md](./CONTRIBUTING.md)** for our `24×24px` Figma grid rules, SVGR pipeline guide, and PR checklist.

---

## 📄 License
All core packages (`@vectui/icons`, `@vectui/tokens`, `@vectui/cli`) and vector assets are open-source under the **[MIT License](./LICENSE)**.