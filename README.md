# ved.blog — Personal Blog

A personal blog built with vanilla HTML, CSS, and JavaScript. Posts are managed through a password-protected admin panel and stored in the browser.

## Host on GitHub Pages

1. Create a GitHub repository
2. Push all files to the repository
3. Go to **Settings → Pages**
4. Under "Branch", select `main` and the `/docs` folder
5. Click **Save**
6. Your blog will be live at `https://yourusername.github.io/repo-name/`

> Note: `docs/index.html` is the deployed page. After editing `index.html`, copy the changes to `docs/index.html` and push.

## File Structure

```
├── index.html              ← Main blog page (edit this)
├── docs/                   ← Deployed copy for GitHub Pages
│   └── index.html          ← Same as index.html (keep in sync)
├── sadhana-tracker.html    ← Standalone tracker (optional)
├── posts/                  ← Legacy files, Notion export sources
├── space-time-fabric.html  ← Legacy standalone page
└── README.md
```

## Features

- **Two tabs**: Posts and About Me
- **Admin panel**: Access with Ctrl+Shift+A (or double-click the logo) and enter the admin password to create, edit, and delete posts
- **Markdown import**: Upload a Notion-exported `.md` file (with its images) directly into a post
- **Likes & comments**: Visitors can like and comment on posts
- **Post storage**: All posts saved in browser localStorage

## How to Run

Open `index.html` in any modern browser. No server needed.

## Tech Stack

| Layer | Technology |
|---|---|
| Structure | HTML5 |
| Styling | Vanilla CSS |
| Interactivity | Vanilla JS + marked.js (CDN) |
| Fonts | DM Serif Display · DM Mono · Inter |
| Storage | localStorage |
| Hosting | GitHub Pages (or any static host) |

*Built with vanilla everything — no frameworks, no build tools.*
