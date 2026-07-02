# Hadi Mustafa Hashmi — Portfolio

A React + Tailwind CSS portfolio site (AI/ML Engineer & Full Stack Developer), built with Vite.

## Structure

```
portfolio-project/
├── index.html            # HTML entry point
├── package.json
├── vite.config.js
├── tailwind.config.js
├── postcss.config.js
├── .gitignore
├── public/                # static assets (empty — all images are embedded as base64 in App.jsx)
└── src/
    ├── main.jsx           # React root
    ├── App.jsx            # the entire portfolio (single component)
    └── index.css          # Tailwind directives + base font styles
```

## Setup

1. Install dependencies:
   ```bash
   npm install
   ```

2. Start the dev server:
   ```bash
   npm run dev
   ```
   Open the printed local URL (usually http://localhost:5173).

3. Build for production:
   ```bash
   npm run build
   ```
   Output goes to `dist/`. Preview it with `npm run preview`.

## Notes

- All images (profile photo, certificate, project logos) and the downloadable CV PDF are embedded directly in `src/App.jsx` as base64 data URIs — no separate asset files needed.
- Skill/tool icons use `react-icons` (Simple Icons set) for real brand logos, plus `lucide-react` for general UI icons.
- Dark/Light mode toggle is built in (top-right nav button).
- To swap the profile photo, certificate, project images, or CV: replace the corresponding `data:...;base64,...` string near the top of `App.jsx`, or refactor to import files from `public/` instead if you prefer real asset files.
- LinkedIn URL in the Contact section (`linkedin.com/in/hadihashmi`) is a placeholder — update it in `App.jsx` if it's not your real profile link.
