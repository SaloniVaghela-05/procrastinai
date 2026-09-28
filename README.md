# ProcrastinAI

A tongue-in-cheek productivity copilot that helps you do it later.

- **Guilt Level gauge** with buttons that raise or lower it (Touch Grass, One More Episode, Actually Do Work)
- **AI Excuse Vault** that types out an overly analytical excuse for any task
- **Someday/Maybe Vortex** where tasks get "Procrastinate Further" tags or get sent to the Tomorrow black hole
- **Slacker Blob** mascot that snoozes, gets vaguely aware, or sweats depending on your guilt

Plain HTML, CSS and JavaScript. No build step, no dependencies, no API keys.

## Run locally

Open `index.html` in a browser. Or serve it:

```bash
python3 -m http.server 8000
# then visit http://localhost:8000
```

## Deploy on GitHub Pages

1. Create a new GitHub repo and push these files to the `main` branch:

   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/<your-username>/procrastinai.git
   git push -u origin main
   ```

2. In the repo, go to **Settings > Pages** and set **Source** to **GitHub Actions**.
3. The included workflow (`.github/workflows/pages.yml`) deploys on every push to `main`. Your site will be live at `https://<your-username>.github.io/procrastinai/`.

Other hosts work too: drag the folder onto Netlify, or import the repo into Vercel (framework preset: Other, no build command).

## Adding a real LLM later

Excuses are generated locally in the `#gen` click handler in `index.html`. To use an LLM, send the task text to your own backend (never put an API key in client code) and use the response in place of the local text. Keep the local generator as a fallback if the request fails.

## License

MIT
