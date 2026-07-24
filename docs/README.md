# ved.blog — Personal Blog

A professional personal blog built with vanilla HTML, CSS, and JavaScript. Posts are managed through a password-protected admin panel and stored in the browser.

## Host on GitHub Pages

1. Create a GitHub repository (e.g., `ved.github.io` or `myblog`)
2. Push all files to the repository
3. Go to **Settings → Pages**
4. Under "Branch", select `main` and `/ (root)` folder
5. Click **Save**
6. Your blog will be live at `https://yourusername.github.io/repo-name/`

## File Structure

```
├── myblog.html              ← Main blog page (open this)
├── sadhana-tracker.html     ← Standalone tracker (optional)
├── posts/                   ← Legacy post files (not linked from main)
├── space-time-fabric.html   ← Legacy standalone page
└── README.md
```

## Features

- **Two tabs**: Posts and About Me
- **Admin panel**: Click "admin" in the footer, enter password `ved2025` to create/edit/delete posts
- **Post storage**: All posts saved in browser localStorage
- **Test post**: A "Hello World" post is pre-loaded as a seed

## Admin Password

Default: `ved2025`

To change it, edit the `ADMIN_PASSWORD` variable in `myblog.html` (line containing `const ADMIN_PASSWORD`).

## How to Run

Open `myblog.html` in any modern browser. No server needed.

## Tech Stack

| Layer | Technology |
|---|---|
| Structure | HTML5 |
| Styling | Vanilla CSS |
| Interactivity | Vanilla JS |
| Fonts | DM Serif Display · DM Mono · Inter |
| Storage | localStorage |
| Hosting | GitHub Pages (or any static host) |

*Built with vanilla everything — no frameworks, no build tools.*
