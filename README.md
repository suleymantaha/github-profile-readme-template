# 🎨 GitHub Profile README Template

A ready-to-use template to make your GitHub profile README stand out. Stats are stored as **local SVG** files and updated via GitHub Actions to avoid rate limits and loading issues.

## 📸 Preview

*Sample SVG output (using suleymantaha's data):*

### Stats
<p align="center">
  <img src="profile/stats.svg" alt="Stats" height="140"/>
  <img src="profile/streak.svg" alt="Streak" height="140"/>
</p>

### Top Languages
<p align="center">
  <img src="profile/top-langs.svg" alt="Top Languages" width="45%" />
</p>

### Achievements & Activity
<p align="center">
  <img src="profile/trophy.svg" alt="Trophies" />
</p>
<p align="center">
  <img src="profile/activity.svg" alt="Activity" width="95%" />
</p>

### Featured Projects
<p align="center">
  <img src="profile/pin-repo1.svg" alt="Pin 1" />
  <img src="profile/pin-repo2.svg" alt="Pin 2" />
</p>

### Contribution Snake
<p align="center">
  <img src="https://raw.githubusercontent.com/suleymantaha/suleymantaha/output/github-contribution-grid-snake-dark.svg" alt="Contribution snake" />
</p>

**[→ View full template](https://github.com/suleymantaha/github-profile-readme-template/blob/main/TEMPLATE_README.md)**

---

## ✨ Features

- 📊 GitHub Stats, Top Languages, Streak
- 🏆 Trophy achievements
- 📈 31-day activity graph
- 📌 Featured project cards (2)
- 🛠️ Tech stack icons
- 🐍 Contribution snake (auto, snake.yml workflow)
- ⏰ Auto-update every 6 hours

## 🚀 Quick Setup

### 1. Use Template

Click **Use this template** to copy this repo. Name the new repo **your username** (e.g. `johndoe/johndoe`) — that's the GitHub profile README format.

### 2. Copy Files

- Rename `TEMPLATE_README.md` → `README.md`
- `.github/workflows/` is already included

### 3. Customize

| Replace | File | Description |
|---------|------|-------------|
| `YOUR_USERNAME` | README.md, workflow | Your GitHub username |
| `YOUR_REPO_1`, `YOUR_REPO_2` | `.github/workflows/update-stats.yml` | Repos to feature |
| Typing lines | README.md | Text in `lines=` param |
| Email, LinkedIn | README.md | Contact info |
| Colors | workflow, README | `title_color`, `icon_color`, etc. |

### 4. First Run

After pushing, trigger the workflow from **Actions** or wait ~6 hours. The `profile/` folder will be populated.

## 📁 Structure

```
.
├── README.md              ← Profile README (from TEMPLATE_README.md)
├── .github/
│   └── workflows/
│       ├── update-stats.yml
│       └── snake.yml
└── profile/               ← SVGs (auto-generated)
    ├── stats.svg
    ├── top-langs.svg
    ├── streak.svg
    ├── trophy.svg
    ├── activity.svg
    └── pin-*.svg
```

## 🐍 Contribution Snake

The included `snake.yml` workflow uses [Platane/snk](https://github.com/Platane/snk) to generate the snake SVG on the `output` branch. It appears after the first push or manual trigger.

## 🎨 Color Customization

Edit color codes in the workflow and README:

- `title_color` — Title color
- `icon_color` — Icon color  
- `text_color` — Text color

## 📄 License

MIT — Use freely.

---

**Note:** This template is generic. Customize it with your own username and repos.
