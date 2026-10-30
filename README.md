# Adaptive AIX

**Creating New Communication Waves.**  
From Idea to AI-Powered Business.

**Live site:** [https://adaptiveaix.com](https://adaptiveaix.com)

![CI](https://github.com/AdaptiveAIX/Main-AIX/actions/workflows/ci.yml/badge.svg)

## Screenshot

![Adaptive AIX homepage](public/screenshot.png)

---

## About Adaptive AIX

Adaptive AIX is an AI-native company that turns real market problems into automated, scalable digital businesses.

Most companies treat AI as a feature or a project. Adaptive AIX treats it as infrastructure. The quality of the system determines the quality and speed of the businesses created.

The company operates a Dual Engine model:

- **Internal** — builds its own portfolio of AI-powered products.
- **Client** — helps selected founders and organizations move from idea to an operational AI-powered business using the same proven system.
- **White-label layer** — successful internal products can be offered as ready-made capabilities so clients do not start from zero.

This creates structural leverage: build once, refine through real use, and extend the capability to clients.

The public website expresses the Dual Engine, the six operating principles, and the eight-step cycle. The internal Operating System is how the company actually runs.

## Tech stack

- **Frontend:** React 19 + Vite
- **Styling:** Custom CSS
- **Hosting:** Cloudflare Pages
- **Domain:** adaptiveaix.com (www redirects to apex)
- **Backend / data (future):** Supabase (project `prvmopjnqmwhjqouqbtm`)
- **Repository:** AdaptiveAIX/Main-AIX

## Local development

```bash
npm install
npm run dev
```

## Deployment

- **Production branch:** main
- Cloudflare Pages automatically deploys every merge to main
- **Build command:** `npm run build`
- **Output directory:** `dist`
- **Live URL:** [https://adaptiveaix.com](https://adaptiveaix.com)

## Architecture notes

The site is a static Vite + React application.

Supabase is prepared in the project (`.env.example` and a small client file) but is not yet used by the public website.

The primary Supabase project is intended as the central Adaptive AIX space for future client projects, internal tools, and later website features.

## Development workflow

1. Create a feature branch from main.
2. Make changes and verify locally with `npm run dev`.
3. Open a pull request into main.
4. After merge, Cloudflare Pages deploys automatically.

## Repository structure

```
├── public/                 # Static assets (logo, favicon)
├── src/
│   ├── App.jsx             # Main application
│   ├── main.jsx            # Vite entry
│   ├── styles.css          # Global styles
│   └── adaptive-aix/       # Future Supabase client (prepared)
├── .cursor/rules/          # Cursor workflow rules
├── index.html
├── package.json
└── vite.config.js
```

## Contact

- Website: https://adaptiveaix.com
- Email: adaptiveaix@gmail.com

## License

Private — Adaptive AIX. All rights reserved.
