# Kunal Meher — GitHub Profile Setup

This package is prepared for the special GitHub profile repository:

`kunalmeher243/kunalmeher243`

## 1. Create the repository

1. Open GitHub and create a **new public repository**.
2. Set the repository name to exactly `kunalmeher243`.
3. Do **not** initialize it with a README.

## 2. Push the profile

Open PowerShell / Git Bash in this folder and run:

```bash
git init
git add .
git commit -m "Create GitHub profile"
git branch -M main
git remote add origin https://github.com/kunalmeher243/kunalmeher243.git
git push -u origin main
```

If Git says the remote already exists, use:

```bash
git remote set-url origin https://github.com/kunalmeher243/kunalmeher243.git
git push -u origin main
```

## 3. Run the GitHub Actions

Open the repository on GitHub → **Actions**.

Run these workflows manually once:

- **Generate Contribution Snake**
- **Generate GitHub Metrics**

The snake workflow publishes its SVG files to the `output` branch. The metrics workflow updates `profile/metrics.svg` on `main`.

## 4. Important

The profile uses third-party public SVG services for typing text, badges, GitHub statistics, streak statistics, and technology icons. These services do not require secrets in the repository.

The GitHub Actions workflows use the repository's built-in `GITHUB_TOKEN`; no personal access token is embedded in this project.
