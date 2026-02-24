# ΧΑΨΙΑ — The Street Food Project

Static website for Hapsia street food, Pangrati, Athens.

## Setup

1. Replace the logo placeholder in `index.html` with your actual logo image (put it in `assets/logo.png`)
2. Update phone number, email, address, and opening hours in `index.html`
3. Replace `assets/menu.pdf` with the latest menu whenever needed

## Deploy

### GitHub Pages

```bash
git init
git add .
git commit -m "initial"
git remote add origin <your-repo-url>
git push -u origin main
```

Then enable GitHub Pages in repo Settings → Pages → Source: main branch.

### S3

```bash
aws s3 sync . s3://your-bucket-name --exclude ".git/*"
```

Enable static website hosting on the bucket.
