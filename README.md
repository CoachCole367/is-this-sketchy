# Is this sketchy?

A simple static webpage that lets you paste a raw email header and get a heuristic "sketchiness" score with the main reasons, recommended next action, and extracted header values.

## Local use

Open `index.html` in a browser and paste a full email header.

## GitHub Pages

Suggested repository name: `is-this-sketchy`

This project is already structured for GitHub Pages because the site entry point is the root `index.html`.

### Publish steps

1. Create a new GitHub repository named `is-this-sketchy`.
2. Push this folder to GitHub.
3. In the GitHub repository, open `Settings` -> `Pages`.
4. Set the source to `Deploy from a branch`.
5. Select the `main` branch and the `/ (root)` folder.
6. Save, then wait for the Pages URL to be published.

### Example push commands

```bash
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/YOUR-USERNAME/is-this-sketchy.git
git push -u origin main
```

## Files

- `index.html`: app UI and scoring logic
- `.nojekyll`: prevents Jekyll processing on GitHub Pages
- `.gitignore`: ignores local Mac metadata files

## Notes

This is a heuristic checker, not a forensic verdict. A low score does not guarantee safety, and a high score does not prove malicious intent.
