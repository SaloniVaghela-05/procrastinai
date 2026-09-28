<div align="center">

# 😴 ProcrastinAI

### The smart copilot that helps you do it later.

*Other productivity apps want you to do things. This one understands you.*

**[Live Demo](https://procrastinai.vercel.app/)** &nbsp;•&nbsp; **[Report a Bug](../../issues)** &nbsp;•&nbsp; **[Request a Feature (eventually)](../../issues)**

![HTML](https://img.shields.io/badge/HTML-CSS-JS-a855f7?style=for-the-badge)
![Dependencies](https://img.shields.io/badge/dependencies-0-a3e635?style=for-the-badge)
![Build step](https://img.shields.io/badge/build%20step-none%20(too%20much%20effort)-ff3d9a?style=for-the-badge)
![License](https://img.shields.io/badge/license-MIT-lightgrey?style=for-the-badge)

</div>

---

## 🤔 What is this?

ProcrastinAI is a satirical (yet weirdly functional) productivity app for people who have 47 tabs open and a deadline in 6 hours.

Instead of fighting procrastination with rigid to-do lists and guilt, it **leans all the way in**. It gives you a guilt gauge, a machine that writes fancy excuses for you, a black hole for your tasks, and a small blob who suffers alongside you.

It is one HTML file. No install, no build, no API keys. Even the setup respects your time.

## ✨ Features

### 📈 The Guilt Level Gauge
A bouncy progress bar that tracks how bad things are. Hit the buttons and watch your status change:

| Button | What it does | Guilt |
|---|---|---|
| 🌱 **Touch Grass** | Fresh air is a valid excuse for two hours | ⬇️ −15 |
| 📺 **One More Episode** | You said that three episodes ago | ⬆️ +12 |
| 💼 **Actually Do Work** | Who are you? Why are you like this? | ⬇️ −25 |

Your rank climbs from **Professional Menu-Browser** all the way up to **3 AM Panic Architect**. Guilt also creeps up by itself while you sit there, because time is a flat circle and so is your inbox.

### 🧠 The AI Excuse Vault
Type a task you're avoiding. Get back a dignified, quasi-academic reason for not doing it, typed out live:

> *"After careful consideration of the literature, the alignment of Mercury and my inbox makes focus inadvisable. Therefore "Write research paper" must wait, for science."*

Thousands of unique combinations. Zero of them are real research.

### 🌀 The Someday/Maybe Vortex
A task list with no **Complete** button. Only two options:

- **Procrastinate Further** adds a tag like *"Deferred to 3 AM panic session"* or *"Rescheduled to a Tuesday that never comes"*.
- **Send to Tomorrow** spins your task into a black hole. It is never seen again.

### 🫠 The Slacker Blob
A sleepy SVG mascot that reacts to your life choices:

| Guilt | Blob mood |
|---|---|
| Low | 😴 Snoozing, with little floating Zs |
| Medium | 😐 Vaguely aware |
| High | 😰 Sweating profusely, shaking |

Every task you delay makes the blob a little bigger. It's fine. It's comfortable.

## 🛠️ Make It Yours

Everything lives in `index.html`, so you can tweak it without any tooling.

| Want to change... | Look for |
|---|---|
| The excuse recipe | the `starts`, `mids` and `ends` arrays |
| Procrastination tags | the `tags` array |
| How much each button moves guilt | the `delta` object |
| Guilt level names and messages | the `levels` array |
| Button quips | the `lines` object |
| Colors | the CSS variables at the top of `<style>` |

Dark neon is the default, and there's an automatic light theme that follows your system setting.


## 🗂️ Project Structure

```
procrastinai/
├── index.html                  # The entire app
├── README.md                   # You are here (finally)
├── LICENSE                     # MIT
├── .nojekyll                   # Tells GitHub Pages to skip Jekyll
└── .github/workflows/
    └── pages.yml               # Auto-deploy to GitHub Pages
```

## 🔮 Roadmap

We will get to these. Eventually. Probably.

- [ ] Save tasks between visits (planned for tomorrow)
- [ ] Sound effects for the black hole
- [ ] More blob moods and skins
- [ ] Drag-and-drop tasks into the black hole
- [ ] Real LLM excuses via a backend
- [ ] Finish the roadmap

## 🤝 Contributing

Pull requests are welcome, especially ones with better excuses. Open an issue or fork the repo. Please keep contributions:

- funny,
- dependency-free where possible,
- and accessible (keyboard focus and reduced-motion support matter, even here).

If your PR takes more than a week to submit, that's on brand and we respect it.

## 📜 License

MIT. Do whatever you want with it, just not right now.

---

<div align="center">

Made with 💜 and a suspicious amount of avoidance.

*If you read this whole README instead of doing your actual work, the app is working as intended.*

</div>
