# Graston Command Center 🚀

The **Graston Command Center** is the all-in-one internal dashboard for events, clinician directory, and marketing automation.

## 🏗 Monorepo Structure
- **apps/**
  - `staff-hub`: Events + Marketing dashboard
  - `provider-directory`: Clinician 360 directory
  - `experiments`: Cloudflare worker sandbox
- **packages/**
  - `ui`: Shared React UI components
  - `api-client`: API wrappers (WooCommerce, FluentCRM, WP Fusion, GTED plugin)
  - `utils`: Utilities (formatting, % full, etc.)
  - `config`: Shared configs (Tailwind, ESLint, TS)

## 🚀 Getting Started
```bash
pnpm install
pnpm dev
```

- Visit `http://localhost:3000` for Staff Hub
- Visit `http://localhost:3001` for Provider Directory

## 🧩 Deployment
- **Staff Hub & Directory** → [Vercel](https://vercel.com/)
- **Experiments** → [Cloudflare Workers](https://developers.cloudflare.com/workers/)

## 🔑 Notes
- Requires WordPress plugin endpoints:
  - `/wp-json/gcc/v1/events`
  - `/wp-json/gcc/v1/marketing/...`
  - WooCommerce, FluentCRM, WP Fusion REST enabled
- Adobe Express Client ID required for Creative Editor
