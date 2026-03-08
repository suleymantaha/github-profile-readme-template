# 📋 Setup Guide

## Step 1: Create Repo

1. Click **Use this template** to copy this repo
2. New repo name: **`yourusername`** (same as your GitHub username)
3. Create as Public

> ⚠️ For GitHub profile README, the repo name must match your username (e.g. `johndoe/johndoe`)

## Step 2: Prepare Files

```bash
# Copy TEMPLATE_README.md to README.md
cp TEMPLATE_README.md README.md
```

## Step 3: Replace Placeholders

### In README.md:

| Placeholder | Replace With | Example |
|-------------|--------------|---------|
| `YOUR_USERNAME` | Your GitHub username | `johndoe` |
| `YOUR_EMAIL` | Your email | `john@example.com` |
| `YOUR_LINKEDIN` | LinkedIn username | `johndoe` |
| `YOUR_REPO_1` | 1st featured project | `awesome-project` |
| `YOUR_REPO_2` | 2nd featured project | `another-project` |

### Typing animation

Edit the text in the `lines=` param. Lines are joined with `+`, separated with `;`:

```
lines=First+line;Second+line;Third+line
```

### In .github/workflows/update-stats.yml:

| Placeholder | Replace With |
|-------------|--------------|
| `YOUR_REPO_1` | First featured repo name |
| `YOUR_REPO_2` | Second featured repo name |

> `username` is auto-filled (`${{ github.repository_owner }}`) — in profile repo format, owner = your username.

## Step 4: First Push & Workflow

1. Commit and push your changes
2. Go to **Actions** → **Update Profile Stats** → **Run workflow**
3. Wait 2–3 minutes
4. The `profile/` folder will be filled with SVG files

## Step 5: Contribution Snake (Automatic)

The included `snake.yml` workflow creates the `output` branch and generates the snake SVG after the first push. If `YOUR_USERNAME` is set in README, the snake will show automatically. To trigger manually: **Actions** → **Generate Snake** → **Run workflow**.

## Troubleshooting

**SVGs not showing?**  
→ Check that the workflow completed successfully in Actions. Review logs if it failed.

**Pin cards empty?**  
→ Ensure `YOUR_REPO_1` and `YOUR_REPO_2` are your existing public repos.

**Trophy not loading?**  
→ We use `gh-trophy.cdnsoft.net` as an alternative. If issues persist, try [ryo-ma/github-profile-trophy](https://github.com/ryo-ma/github-profile-trophy) load balancing URLs.
