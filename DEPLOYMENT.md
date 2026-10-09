# Artroom browser deployment

## Vercel project settings

- Git repository: `gearsganesh/Artroom`
- Production branch: `main`
- Root Directory: repository root (`.`); do not set it to `frontend/apps/artcraft`
- Framework Preset: Other
- Install Command: `cd frontend && npm ci`
- Build Command: `cd frontend && npm run build --workspace=artcraft`
- Output Directory: `frontend/apps/artcraft/dist`

This builds the Vite frontend. A successful static build alone does not guarantee that every feature designed for the Tauri desktop host is functional in a normal browser. Verify login, API configuration, and host-specific functionality before production release.
