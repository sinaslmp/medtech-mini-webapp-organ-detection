# MedTech Organ Detection — Frontend

[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue?style=flat-square&logo=github)](https://sinaslmp.github.io/medtech-mini-webapp-organ-detection/)
[![Vue](https://img.shields.io/badge/Vue-3-4FC08D?style=flat-square&logo=vue.js&logoColor=white)](https://vuejs.org)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://typescriptlang.org)
[![Vite](https://img.shields.io/badge/Vite-5-646CFF?style=flat-square&logo=vite&logoColor=white)](https://vitejs.dev)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)

A MedTech frontend application for medical image analysis and organ detection, built as an extension of the [medtech-mini-webapp](https://github.com/sinaslmp/medtech-mini-webapp) project. The frontend is deployed on **GitHub Pages** and connects to a FastAPI backend for image processing.

---

## Features

- Upload medical images (JPG / PNG) for analysis
- Select and apply image processing phases (arterial / venous)
- Organ detection and analysis UI
- Side-by-side comparison of original and processed images
- Responsive design — works on mobile, tablet, and desktop
- CI/CD pipeline via GitHub Actions (automatic deploy to GitHub Pages)

---

## Live Demo

**Frontend:** [sinaslmp.github.io/medtech-mini-webapp-organ-detection](https://sinaslmp.github.io/medtech-mini-webapp-organ-detection/)

**Backend:** See [medtech-mini-webapp](https://github.com/sinaslmp/medtech-mini-webapp) for the FastAPI image processing API.

---

## Tech Stack

| Layer | Technology |
|---|---|
| Framework | Vue 3 + Composition API |
| Language | TypeScript 5 |
| Build Tool | Vite 5 |
| CI/CD | GitHub Actions |
| Hosting | GitHub Pages |

---

## Local Development

### Prerequisites

- Node.js ≥ 18
- npm ≥ 9

### Setup

```bash
# Clone the repository
git clone https://github.com/sinaslmp/medtech-mini-webapp-organ-detection.git
cd medtech-mini-webapp-organ-detection

# Install dependencies
npm install

# Configure environment
cp .env.example .env
# Edit .env and set VITE_BACKEND_URL to your FastAPI backend URL

# Start development server
npm run dev
```

Open http://localhost:5173 in your browser.

### Build for Production

```bash
npm run build
```

Output is in the `dist/` folder.

---

## Project Structure

```
medtech-mini-webapp-organ-detection/
├── .github/workflows/      # GitHub Actions CI/CD (auto-deploy to Pages)
├── public/                 # Static assets
├── src/
│   ├── assets/             # Images and styles
│   ├── components/         # Vue components
│   ├── App.vue             # Root component
│   ├── main.ts             # App entry point
│   └── style.css           # Global styles
├── .env.example            # Environment variable template
├── .gitignore
├── index.html
├── package.json
├── tsconfig.json
└── vite.config.ts
```

---

## Environment Variables

| Variable | Description | Example |
|---|---|---|
| `VITE_BACKEND_URL` | FastAPI backend base URL | `https://sinaslmp-medtech-phase-backend.hf.space` |

---

## Related Projects

- [medtech-mini-webapp](https://github.com/sinaslmp/medtech-mini-webapp) — Original full-stack version (Vue + FastAPI) with complete backend and README

---

## License

MIT — free to use and modify.
